# day-05

3) programs in arrow function :-
  a)print odd numbers in an array :
                       let arr = [1,2,3,4,5,6,7,8,9,10,11,12]
                       let oddnumbers = arr.filter(n => n%2)
                       console.log(oddnumbers);	
  b)convert all the strings to title caps in an array :
                       function title (str) {
                       return str .split(' ').map((word) => word.toUpperCase()).join(' ')
                         };
                       console.log(title("Vigneshwar BE Mechanical Engineering"));
 c)sum of numbers in an array :
                       let arr = [22,24,55,64];
                       let sum = arr.reduce((a,b) => a+b);
                       console.log(sum);

 d)return all the prime numbers in an array :
                       const arr= [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18];
                       const prime = arr.filter(num => {
                       for (let i = 2; i < num; i++) {
                       if (num % i === 0) 
                                 return false;
                       }
                       return num !== 1;
                       });
                       console.log(prime);
           

 e)return all palindromes in an array :
                      let getfirst = (firstName,middleName,lastName) => {
                              return firstName.charAt(0) + middleName.charAt(0)+lastName.charAt(0);
                              };
                      console.log(getfirst("Charlie","Suresh", "Brown"));
                      
                      
                      
                      2) programs in anonymous function and iife functions :
a)odd numbers :
    1) arrow function:       
             let arr=[1,2,3,4,5];
                   let odd = function () {
                   let odd= arr.filter(num => num %2 ==1)
                   console.log(odd)
                   }
                   odd()
     2) iife function :
                    let a=[0,1,2,3,4,5,6,7,8,9];
                   (function ()  {
                   let odd= a.filter(num => num %2 ==1);
                   console.log(odd)
                  })();
b)string in title caps :
      1) anonymous function :     
                  var str = toTitles('hi i am vignesh menon');
                  function toTitles(s){ return s.replace(/\w\S*/g, function(t) { 
                  return t.charAt(0).toUpperCase() + t.substr(1).toLowerCase(); 
                  }); }            console.log(str);  
