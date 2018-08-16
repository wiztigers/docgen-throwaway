<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Amazing Book</title>
</head>
<body>
<script>
  var lang = navigator.language || navigator.userLanguage;
  if (lang.indexOf('fr') == 0)
       window.location = {% assign new_redirect_fr = site.url | append: '/fr/' %};
  else window.location = {% assign new_redirect_en = site.url | append: '/en/' %};
</script>
</body>
</html>
