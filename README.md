<html>
    <head>
        <meta charset="utf-8">
        <title>New webpage</title>
        <style>
            button{
                background-color:white;
            }
        </style>
    </head>
    <body>
        <div style="overflow:auto; height: 200px;width:50%;">
            <button onClick="buy('party time');">party time:<br>20</button>
            <button onClick="buy('smily');">smily:<br>19</button>      
            <button onClick="buy('mounain man');">mounain man:<br>17</button>
            <button onClick="buy('clif hanger');">clif hanger:<br>17</button>          
            <button onClick="buy('plain');">plain:<br>14</button>
        </div>
        <div id="ord">Order:</div>
        <span id="price"></span>
<input type="button" value="Print Order" onclick="printPage()" />
        <script>    
            var price =0;    
            function buy(type){                
                if(type==='mounain man'){
                    document.getElementById("ord").innerHTML+="<br>mounain man price: 17";
                    price=price+ 17;
                    document.getElementById("price").innerHTML=price;
                }else if(type==="clif hanger"){
                    document.getElementById("ord").innerHTML+="<br>cliff hanger price: 17";
                    price=price+ 17;
                    document.getElementById("price").innerHTML=price;
                }else if(type==='smily'){
                    document.getElementById("ord").innerHTML+="<br>smily price: 19";
                    price=price+ 19;
                    document.getElementById("price").innerHTML=price;
                }else if(type==='party time'){
                    document.getElementById("ord").innerHTML+="<br>party time price: 20";
                    price=price+ 20;
                    document.getElementById("price").innerHTML=price;
                }else if(type==='plain'){
                    document.getElementById("ord").innerHTML+="<br>plain price: 14";
                    price=price+ 14;
                    document.getElementById("price").innerHTML=price;
                }         
            }
            function printPage() {
  window.print();
}
        </script>
    </body>
</html>
