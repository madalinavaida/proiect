<script>
  allCookies = document.cookie;
  document.cookie = "test1=Hello";
  document.cookie = "test2=World";

const cookieValue = document.cookie
  .split('; ')
  .find(row => row.startsWith('test2='))
  .split('=')[2];

function alertCookieValue() {
  alert(cookieValue);
}
</script>
<body> Bine ai venit la lab 
  <button onclick="alertCookieValue()">Show cookie value</button>
</body>
