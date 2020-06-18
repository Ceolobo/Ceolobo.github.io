---
layout: base
title: PYTest
---

<html>
<body>

<h1>My First Web Page</h1>
<p>My First Paragraph</p>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = 5 + 6;
</script>

<p> Second Paragraph</p>

<p id="demo2"></p>

<script>
$.ajax({
   url: "/test.py",
   success: function(response) {
     document.getElementById("demo2").innerHTML = response;
   }
});
</script>

</body>
</html>
