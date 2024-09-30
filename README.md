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
            localStorage.setItem('ARCoder.org', document.getElementById('s').value);
            function saver (){
                localStorage.setItem('ARCoder.org', document.getElementById('s').value);
            }
            function look (){
                var page = document.getElementById("address").value;
                if(page==="gobble.anti"){
                    document.getElementById("page").innerHTML="";
                }else if(page==="ARCoder.org/***"){
                    document.getElementById("page").innerHTML="<textarea id='s' value="+localStorage.getItem('ARCoder.org')+"></textarea><button onclick='saver()'>save</button>";                    
                }else if(page==="ARCoder.org"){
                    document.getElementById("page").innerHTML=localStorage.getItem("ARCoder.org");
                }
            };
        </script>
    </body>
</html>

