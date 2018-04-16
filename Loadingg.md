<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1" />
<title>Tes Jquery Progress</title>
<link type="text/css" href="css/black-tie/jquery-ui-1.8.21.custom.css" rel="stylesheet" />
  <script type="text/javascript" src="js/jquery-1.7.2.min.js"></script>
  <script type="text/javascript" src="js/jquery-ui-1.8.21.custom.min.js"></script>
<style type="text/css">
<!--
body {
 background-color: #6da5ff;
}
-->
</style>
</head>
<script type="text/javascript">
  var proses=0;
  var henti=0;
  $(document).ready(function(){
mulai();
});
   function mulai(){
   myVar=setInterval(function(){tambahProses()},100);
   }
 function tambahProses(){
  if(proses >= 100 ){
   henti=0;
   clearInterval(myVar)
   window.location.assign("https://itk.ac.id")
   }else{
  proses+=1;
  $( "#progressbar" ).progressbar({
   value:  proses
      });
    }
 }
  </script>
<body>
<fieldset>
<h1>Tunggu sedanag proses.. </h1>
<div id="progressbar">
</div>
<div style="display: none;" class="demo-description">
<p>Default determinate progress bar.</p>
</div>
<table width="173" border="0" align="center">
</table>
<p align="center"> </p>
<p> </p>
</fieldset>
</body>
</html>
