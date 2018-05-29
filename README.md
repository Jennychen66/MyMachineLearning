# MyMachineLearning

    I got a notification for TensorFlow.js one day, this reminds me a lot of new thinking over machine learning domain. 
    And I'm also start looking for a job on this machine learning area, 
    I think it isn't much harder when I have a mathematical background as well as several years' experience on computer vision.

The material record for my learning 
1. The official website of Tensorflow.js https://js.tensorflow.org/ 
2. 


- - - 
###  How to compile and build a Javascript code from a command line

    1) we can use babel to compile Javascript, the official site is http://babeljs.io/docs/setup/#installation 
    2) Install 
        I) create a package.json in your folder which you want to install the babel , and you can add the code 
`{
           "devDependencies": {}
 }`
         
         run the command line 
`npm install --save-dev babel-cli`

   You can also folow the 2-3 steps of this link http://babeljs.io/docs/setup/#installation , it's the same with what I was saying up there.

    II) follow the 4. configration step of this link https://blog.csdn.net/suwu150/article/details/77198968 , after that we can convert ES6 to compile as ES5.
    III) Add a tensorflow.js file inside a js foler inside this project folder , add the following code 
`var num = [1, 2, 3, 4];  
var plusDouble = num.map(function (item) {  
  return item * 2;  
});  
console.log(plusDouble);
let num1 = [1,2,3,4];  
let plusDouble1 = num1.map(item => item * 2);  
console.log(plusDouble);`
    
    run the command line from command prompt :
`./node_modules/.bin/babel-node ./js/tensorTest.js`

    You can see the following results :
`[ 2, 4, 6, 8 ]
[ 2, 4, 6, 8 ]
`
