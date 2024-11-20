<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="content-type" content="text/html; charset=utf-8" />
    <meta name="" content="">
    <title>text changer</title>
    <style type="text/css" media="all">
      *{
        margin: 0;
        padding: 0;
      }
      .container{
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        
      }
      .box{
        width: 500px;
        height: 500px;
        
      }
      .text{
        text-align: center;
        text-transform: capitalize;
        margin: 2rem;
        text-transform: uppercase;
      }
      .btns{
        display: grid;
        grid-template-columns: repeat(2,1fr);
      }
      .button{
        padding: 2rem;
        margin: 1rem;
        text-transform: capitalize;
        font-weight: bold;
        letter-spacing: 2px;
        border: 3px solid ;
        border-radius: 15px;
        font-size: 15px;
       
      }
      .button:hover{
        color: white;
        background: black;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="box">
        <h1 class="text">text color picker</h1>
        <div class="btns">
       <button class="button btn" >red</button>
       <button class="button btn" >orange</button>
       <button class="button btn" >yellow</button>
       <button class="button btn" >green</button>
       <button class="button btn" >blue</button>
       <button class="button btn" >indigo</button>
       <button class="button btn" >violet</button>
       <button class="button btn" >maroon</button>
        </div>
      </div>
    </div>
    <script type="text/javascript" charset="utf-8">
      let text =document.querySelector('.text')
      
      
      let btns =document.querySelectorAll('.btn')
      
      btns.forEach((btn)=>{
        btn.addEventListener('click',()=>{
let value=btn.textContent
text.style.color=value

        })
      })
      
      
    </script>
  </body>
</html>
