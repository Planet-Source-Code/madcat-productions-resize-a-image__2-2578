<div align="center">

## Resize a image


</div>

### Description

This code resize a image by a given factor.
 
### More Info
 
a scaled image


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Madcat Productions](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/madcat-productions.md)
**Level**          |Beginner
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |
**Category**       |[Graphics](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/graphics__2-75.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/madcat-productions-resize-a-image__2-2578/archive/master.zip)





### Source Code

```
<%@ Language=VBScript %>
<HTML>
<HEAD>
</HEAD>
<BODY>
<form name="preview">
 <script language = "JavaScript">
function loadImage(pic,imgname,maxwidth,scalefactor){
	var h
	var w
	var scalefactor
	var maxwidth
	var scalefactor
	var theimg
alert(maxwidth + " " + scalefactor)
	theimg = new Image();
	theimg.src = pic;
	h = theimg.height;
	w = theimg.width;
if (w > maxwidth){
	w = (theimg.width * scalefactor) / theimg.width;
	h = (theimg.height * scalefactor) / theimg.width;
	}
document.writeln("<img src='" + theimg.src +"' name='" + imgname + "' width='" +w+"' height='" +h+"'>");
}
</script>
<%
img = "Product_Images/MicroStation.jpe"
%>
 <META NAME="GENERATOR" Content="Microsoft Visual Studio 6.0">
<script>
loadImage('<%=img%>','imgchange',100,400)
</script>
</form>
</BODY>
</HTML>
```

