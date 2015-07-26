---
layout: post
title: Indian Loksabha - Member Qualification
customjs: https://online.tableau.com/javascripts/api/tableau-2.0.0.min.js
excerpt: Indian polititians usually have a bad reputation when it comes to their education qualifications. So I was wondering if there is some way to summarize that info. This is what I found.
---
Indian polititians usually have a bad reputation when it comes to their education qualifications. So I was wondering if there is some way to summarize that info. This is what I found.


<script>
window.onload = function () {
  var placeholderDiv = document.getElementById("tableauViz");
  var url = "https://public.tableau.com/views/LoksabhaMemberQualification/MemberQualification";
  var options = {
    height: 800,
    hideTabs: true,
    hideToolbar: true,
    onFirstInteractive: function () {
      workbook = viz.getWorkbook();
      activeSheet = workbook.getActiveSheet();
    }
  };
  viz = new tableau.Viz(placeholderDiv, url, options);
} 
</script>

<div id='tableauViz'></div>

The data for this infograph comes from the [this site](http://164.100.47.132/LssNew/Members/breif_alphalist.aspx). I plotted it using [Tableau Public](https://public.tableau.com/s/).

How I extracted the info and how I made this infograph will come in another post.

Please do share your views!
