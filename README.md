<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>9.6</title>
</head>
<body>
	<script>
		var table="<table border=1 cellspacing=0 cellpadding=10>";
		for(var i=1;i<11;i++){
			table=table+"<tr>";
			for (j=1;j<i;j++){
				table=table+"<td align=center>"+i+"-"+j+"</td>";
			}
			table=table+"</tr>";
		}
		document.write(table);

		for (var a=1;a<=9;a++){
			if(a%2==0){
				for (var b=1;b<+a;b++){
					document.write("*")
				}
				document.write("<br>")
			}
		}
		var row=prompt('请输入行数：',6);
		for(var i=1;i<=row;i++){
			for(var j=1;j<=row-i;j++){
				document.write("-");
			}
			for(var j=1;j<=2*i-1;j++){
				document.write("*");
			}
			document.write("<br>");
		}
		var a=1,b=1;
		for(var c=0;c<=100;){
			c=a+b;
			document.write(c+"&nbsp");
			a=b;
			b=c;
		}
		var col=[1,2,3,5,6,7,8,9]
		for(i=0;i<col.length;i++){
			console.log(col[i])
		}
		
	</script>
</body>
</html>
