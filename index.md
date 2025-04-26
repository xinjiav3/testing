---
layout: post
title: Testing Repository
description: A testing repository created for playing around
author: Zhengji Li
---

<html>
<head>
    <title>Testing</title>
    <!-- permalink -->
</head>
<body>
    <h1>Testing</h1>
    <p>Testing</p>
    <form onsubmit="return changeName(event)">
        <input type="text" id="nameInput" placeholder="Enter new name.">
        <input type="submit" value="Save changes">
    </form>
    <div class="result">
        <a href="#" id="headerName">Welcome,<br /> User</a>
    </div>
    <script>
        function changeName(event) {
            event.preventDefault();
            let name = document.getElementById("nameInput").value;
            document.getElementById("headerName").innerText = "Welcome,\n" + name;
            return false;
        }
    </script>
</body>
</html>

