<script>
  allCookies = document.cookie;
  document.cookie = newCookie;
  function doOnce() {
  if (!document.cookie.split('; ').find(row => row.startsWith('doSomethingOnlyOnce'))) {
    alert("Do something here!");
    document.cookie = "doSomethingOnlyOnce=true; expires=Fri, 31 Dec 9999 23:59:59 GMT";
  }
}
</script>
<body> Bine ai venit la lab 
  <button onclick="doOnce()">Only do something once</button>
</body>
