<!DOCTYPE html>
<html>
<head>
<title>Dark Mode Toggle</title>
</head>

<body style="font-family:Arial; text-align:center; margin-top:100px;">

<h1>Dark Mode Toggle</h1>

<button onclick="toggleMode()" style="padding:10px 20px; font-size:18px;">
Toggle Dark Mode
</button>

<script>

let mode = localStorage.getItem("theme");

if(mode === "dark"){
    document.body.style.backgroundColor = "black";
    document.body.style.color = "white";
}

function toggleMode(){

    if(document.body.style.backgroundColor === "black"){
        document.body.style.backgroundColor = "white";
        document.body.style.color = "black";
        localStorage.setItem("theme","light");
    }
    else{
        document.body.style.backgroundColor = "black";
        document.body.style.color = "white";
        localStorage.setItem("theme","dark");
    }

}

</script>
<script src="script.js"></script>

</body>
</html>
