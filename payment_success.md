---
title: Rad! Here's your code
layout: bare
description: Payment Success
showinnavmenu: false
---

<div id="dynamic-content"></div>

<script>

$( document ).ready(function() {
  $.each(document.location.search.substr(1).split('&'),function(c,q){
      var i = q.split('=');
      if (decodeURIComponent(i[0].toString()) === 'code') {
        var code = decodeURIComponent(i[1].toString());
        $("#one .inner .major h1").text('Rad! Here\'s your code: '+code);
        $("#dynamic-content").append('<h3>Send a text message with \'add '+code+'\' to (505) 384-7674 </h3>');
        $("#dynamic-content").append('Please be sure to send this code right away; you\'ll only see this code once');
      }
    });
});

</script>