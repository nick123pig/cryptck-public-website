---
title: Check Your Phone!
layout: bare
description: Get started!
showinnavmenu: false
---

<div id="dynamic-content"></div>

<script>

$( document ).ready(function() {
  $.each(document.location.search.substr(1).split('&'),function(c,q){
      var i = q.split('=');
      if (decodeURIComponent(i[0].toString()) === 'message') {
        $("#dynamic-content").append(decodeURIComponent(i[1].toString()));
      }
    });
});

</script>