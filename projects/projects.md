  
# Projects Related for Dom

## project Link 
[click here]()


# solution code 

## project 1 

```javascript
const bottons = document.querySelectorAll('.button');
const body = document.querySelector('body');

console.log(bottons);

bottons.forEach(function (button) {
  //console.log(button);
  button.addEventListener('click', function (e) {
    console.log(e);
    console.log(e.target);

   switch(e.target.id)
   {
     case 'grey':
       body.style.backgroundColor = e.target.id;
       break;
     case 'white':
       body.style.backgroundColor = e.target.id;
       break;
     case 'blue':
       body.style.backgroundColor = e.target.id;
       break;
     case 'yellow':
       body.style.backgroundColor = e.target.id;
       break;

       default :
         console.log("color not available")
   }
  });
});

```

##project 2

```javascript

 
 const from=document.querySelector('form')

 from.addEventListener('submit',function(e){
       e.preventDefault();

       const height=parseInt(document.querySelector('#height').value)
       const weight=parseInt(document.querySelector('#weight').value)
       const results=document.querySelector('#results')

       if(height === '' || height<0 || isNaN(height)){

            results.innerHTML=`Enter valid Number ${height}`

       }else if(weight === '' || weight < 0 || isNaN(weight)){

            results.innerHTML=`Enter valid Number ${weight}`

       }else{
         const bmi=(weight / ((height * height) / 10000)).toFixed(2);

         results.innerHTML=`<span>${bmi}</span>`;
       }
 });

```