# problem
Great repository names are short and memorable. Need inspiration? How about musical-eureka?

let sentence =
"learn with Sumit is all about teaching web development skills and techniques in an efficient and practical manner. if you are just getting started in web development, Learn with Sumit has all the tools you need to learn the newest and most popular technologies to convert you from a no-stack to a full-stack developer. Lear with Sumit also deep dives onto advanced topics using the latest best practices for you seasoned web developer.";

let someText = sentence.match(/sumit/gi);
let someArray = someText ? someText.length : 0;
console.log(someArray);

let position = sentence.search(/sumit/i);
 position = position >= 0 ? position : "Not found";

console.log(position);

// 1st problem solution


function linearSearch(arr, val){
    let length = arr.length;
    for(let i = 0; i < length; i++){
        if(arr [i] === val){
            return i;
        }
    }
    return 'Not found'
  }
  console.log(linearSearch(['a','b','c','d','c'],'c'));

  // 2nd problem solution

  const arr = ['Fardin Fiyaz Druba','Azmain Faiyz Dip','Najmul Hoque Majumder Mithu', 'Nahida Akter Chowdhury', 'Najat Houqu Roja','Nabila Hoque Majumder','Ikhtiar Uddin Mohhamad Bin Bokhtiar Khilji']


  function Find(arr){
   const newArr = []
   let index  = 0 
  
   for (var i = 0; i < arr.length; i++){
      newArr[index] = arr[i].length
      index++
      
   }
  
  var max = Math.max(...newArr)
  var indexMAx = newArr.indexOf(max)
  
  console.log('Longest name length is of ' + arr[indexMAx] + ' length is ' + max + ' in index ' + indexMAx) 
  }
  
  Find(arr)

  // 3rd problem solution

  function fizzBuzz (number) {

    for(let i = 1; i <= number; i++){
        if(i % 15 === 0){
            console.log(`${i} is FizzBuzz`);

        } else if(i % 3 === 0){
            
                console.log(`${i} is Fizz`);  
        
    } else if(i % 5 === 0){

        console.log(`${i} is Buzz`);

    }
     else{
        console.log(i); 
    }

  }
}
fizzBuzz(100);

// 4th problem solution
const mixedArr = [
    'Iws',
    undefined,
    'learn with sumit',
    false,
     "",
     'apple',
     40,
     "k",
     true,
     'Thanks all',
     NaN
];

const trueArray = mixedArr.filter(Boolean);

console.log(trueArray);

// 5th problem solution
const obj = {
    a: 'Iws',
    b: undefined,
    c: 'learn with sumit',
    d: false,
    e: "",
    f: 'apple',
    g: 40,
    h:  "k",
    i: true,
    j: 'Thanks all',
    k: NaN,
};

const truworthyobject = function(obj){
    for(let i in obj){
        if(!obj[i]){
            delete obj[i];
        }

    }
    return obj;
}

console.log(truworthyobject(obj));
