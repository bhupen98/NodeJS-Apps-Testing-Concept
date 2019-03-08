## Why Testing is so important
 1. Saves time
 2. Creates Realiable Software
 3. Gives flexible to developers
 4. Refactoring
 5. callaborating
 6. Profiling
 

## Testing frameworks
  Test could be using many frameworks like mocha, expresso, jsUnit, should, jest etc..</br>
  But this demo would be of jest framework.</br>
  *To install jest from terminal,*
  ```javascript
  npm install jest --save-dev
  ```
  Add the following script in package.json,
  ```json
  "scripts":{
  "test":"jest"
  }
  ```
  Now, type following command inside a working directory to find out, *if jest works or not*.
  ```terminal
  npm test
  ```
  <img src="https://user-images.githubusercontent.com/47861774/54043300-57a88b80-41f4-11e9-8dfa-9662ab5fe8db.png" height="150px" width="500px"/>
  This shows that your jest works perfectly.
  
  ##  first test
  create a file name math.test.js in your working directory,and follow the code below.
  
  ```javascript 
  test('hello world!',()=>{
  });
  ```
  ![test1](https://user-images.githubusercontent.com/47861774/54045335-6fced980-41f9-11e9-9fe3-d2c5f29b4031.png)
   
   In the above figure you would notice that the jest still inform us about the file pass, eventhought the function does absolutly nothing, **Why is that?**</br>
   When registering a test, we call a test function providing a name and the function.</br>
  when jest runs our test, it simply runs that function, if the test throws an error then the test is considered to be a failure else it is considered to be  success.</br>
          
  Let's add a test to be failure,
  
   ```javascript 
  test('it should fail!',()=>{
  throw new Error('failure');
  });
  ```
  ![test3](https://user-images.githubusercontent.com/47861774/54047248-ab1fd700-41fe-11e9-894a-4d8296b05bb2.png)
  
 In the above figure,jest proves 'it should fail' a failure. It also shows the adject line of failure and more details.
 
 This simple principal is gonna be expanded in more complex real world scenario.
 

 

       
