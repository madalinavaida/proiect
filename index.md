allCookies = document.cookie;

<script>
  document.cookie = "session=test GDPR"; 
  document.cookie = "favorite_task=collect Data"; 
  function alertCookie() { alert(document.cookie); } 
  document.cookie = newCookie;
  document.cookie = "name=oeschger";
  document.cookie = "favorite_food=tripe";
  function alertCookie() {
  alert(document.cookie);
}
</script>
<body> Bine ai venit la lab 
  <button onclick="alertCookie()">
    Show cookies</button> 
  <button onclick="alertCookie()">Show cookies</button>
</body>
