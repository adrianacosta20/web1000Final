# Final exam

## Instructions

Create a github repository called web1000-final. **If you do not name your repository correctly and don't submit it to canvas you will receive a zero. Looking at you, Arnaldo.**

In your repository, create a file called testAnswers.txt and **copy and paste all the questions in there.**

Answer each question right below the question text.

## Questions

1. What are the four steps of mergesort?

1- split array in 2
2- mergesort left half
3- mergesort right half
4- Join the two arrays

2. Using JavaScript, generate a random number between 50 and 100.

function generate(){
  return ((Math.random() * 100 ) + 50)
}

3. Using Javascript, generate a random number between -100 and 100.

function generate(){
  return ((Math.random() * 100 ) - 100)
}

4. Write a coin flip function. It should return the string "heads" half the time and the string "tails" the other half
```javascript
  function coinFlip(){
    var headTails = ['head','tails'];

    return  result=[Math.floor((Math.random()*headTails.length))]
  }
```

5. Re-state the following expression without using negation:
  !(10 > x)

  // (10 <= x) //

6. Re-state the following expression without using negation:
  !(a > 10 && b <= 5)

  //(a <= 10 && b > 5) //

7. Re-state the following expression without repeating variable a:
  (a && x <= 10) || (a && y < 0)

8. Re-state the following expression without negations:
  !( (a > 10) || (b > 10) || (c > 10) || (isAdmin) )

  // ((a<= 10) || (b<=10) || (c<=10) || (!isAdmin) ) //

9. Write a function which, given a 2-d array of strings, returns the concatenation of all the strings.
```javascript
  function twodconcat(arr){
    for(var i =0; i<arr.length; i++){
      return arr[i] +=
    }
  }
```

10. Write a function which, given a 2-d array and another value x, returns true if x is present in the 2-d array, and false otherwise.
```javascript
  function containsElement(arr, x){
    for(var i = 0; i< arr.length; i++){
      if(arr[i] === x){
        return true
      }else{
        return false
      }
    }

  }
```

11. Write a function which, given an two sorted arrays of sizes m and n, returns a larger sorted array of size m+n. This function must work in O(m+n) time.

```javascript
function conc(m, n){
  return Array.from(new Set([...m,...n]))
}
```

12. Given the following edge list, draw the graph. Use MS Paint and include the file in your repo.

```javascript
E = [[1,2], [2,3], [4,5], [2,4], [1,5]  ]
```

13. Given the following adjacency Matrix, determine whether the graph is directed or undirected and draw it.

```javascript
M = [
  [0,0,1,0,1],
  [0,0,0,0,1],
  [0,1,0,0,0],
  [0,1,0,0,0],
  [0,0,0,0,1],
]
```

14. For exercises 9 and 10, if you assume that n is the size of one side of the matrix, what is the time complexity (Big Oh) of the algorithms you wrote?

15. What is the time complexity of the following function?

```javascript
  function thugPop(arr){
    var ret = [];
    for (var i === 0; i < arr.length; i++){
      if (arr[i] % 15 == 0) ret.push('thugPop');
      else if (arr[i] % 5 == 0) ret.push('thug');
      else if (arr[i] %3 == 0 ) ret.push('pop');
      else ret.push(arr[i]);
    }
    return ret;
  }
```
//O(n+k)Linear//

16. What is the time complexity of the following function?

```javascript
  function thugify(schoolList){
    return schoolList.map(function(schoolObj){
      var school = Object.assign({}, schoolObj);
      school.students.forEach(function(student){
        if (Math.random() > 0.5){
          student.lastName += 'dogg';
        }
        else {
          student.firstName = "lil' "+ student.firstName;
        }
      });
    });
  }
```

//0(n^2)Quadratic//

17. What is the time complexity of the following function?

```javascript
  function countRepeats(strArr){
    var repeats = 0;
    strArr.forEach(function(str, index){
      var currentRepeats = strArr.filter(function(innerStr, idx){
        return (innerStr === str && index != idx)
      });
      if (currentRepeats.length > 0){
        repeats++;
      }
    });
    return repeats;
  }
```
//0(n^2)Quadratic//

18. What are the main operations of a stack?

//push, pop//

19. What are the main operations of a queue?

//enqueue, dequeue//

20. What is the runtime of bubblesort? How does it work?

//O(n^2) it compares the current value to the value next to it to see if it is greater or less than. A swap is made if necessary, then it moves onto the next value and does the same thing. This continues from beginning to end of array until no further swaps can be made.//

21. Create a personal website and upload it so that it is accessible at yourdomain.fvi-grad.com.  
    1. The website must have your name, contact information, skills, and at least two links to portfolio items you are hosting on fvi-grad.
    2. The website must not be in a subdirectory of the document root. ie. It needs to be accessible by going to yourusername.fvi-grad.com/ without anything after the slash.
    3. You can and should use a template
    4. Include the link to your website in your answers document

//http://aacosta.fvi-grad.com/blog///
