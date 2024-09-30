<html>
    <head>
        <style>
            body{ 
                background:black;
                color: green;}
        </style>
    </head>
    <body>
        search the ARCoder web: <input id="address"> <button onClick="look()">search</button>
        <div id="page"></div>
        <script>
            function savera (){
                localStorage.setItem('ARCoder.org', document.getElementById('s').value);
            }
            localStorage.setItem('gobble.anti', document.getElementById('s').value);
            function saverc (){
                localStorage.setItem('gobble.anti', document.getElementById('s').value);
            }
            function look (){
                var page = document.getElementById("address").value;
                if(page==="gobble.anti"){
                    document.getElementById("page").innerHTML="";
                }else if(page==="ARCoder.org/91413"){
                    document.getElementById("page").innerHTML="<textarea id='s' value="+localStorage.getItem('ARCoder.org')+"></textarea><button onclick='savera()'>save</button>";                    
                }else if(page==="ARCoder.org"){
                    document.getElementById("page").innerHTML=localStorage.getItem("ARCoder.org");
                }else if(page==="gobble.anti/6711"){
                    document.getElementById("page").innerHTML="<textarea id='s' value="+localStorage.getItem('gobble.anti')+"></textarea><button onclick='saverc()'>save</button>";                    
                }
            };
        </script>
    </body>
</html>

