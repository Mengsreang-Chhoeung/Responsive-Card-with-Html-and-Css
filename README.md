### Responsive-Card-with-Html-and-Css
#### Enjoy coding with html and css...

លំហាត់ខាងក្រោមនេះ ទាមទារឲ្យអ្នកមានចំណេះដឹងទាក់ទងនឹង:
- HTML
- CSS
  - Flexbox
  - Media Query
 
# លំហាត់ Responsive Card
![Thumbnail](https://i9.ytimg.com/vi/DPmNqNWmZP0/maxresdefault.jpg?time=1605348900000&sqp=CKTcvv0F&rs=AOn4CLAZM9n2Na7rXDuETnIrXxDOogiXkw)
# កូដ HTML:
```javascript
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<title>MengSreang Channel</title>
	<link rel="stylesheet" type="text/css" href="css/style.css">
	<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css">
</head>
<body>
	<div class="container">
		<div class="image">
			<img src="https://images.pexels.com/photos/70497/pexels-photo-70497.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" alt="hamburgar">
		</div>
		<div class="content">
			<h1 class="title">Hamburgar</h1>
			<p class="paragraph">
				Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
				tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
				quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
				consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
				cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
				proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
			</p>
			<span>
				<i class="fas fa-star" style="color: #E74C3C;"></i>
				<i class="fas fa-star" style="color: #E74C3C;"></i>
				<i class="fas fa-star" style="color: #E74C3C;"></i>
				<i class="fas fa-star" style="color: #E74C3C;"></i>
				<i class="fas fa-star" style="color: #E74C3C;"></i>
				&nbsp;
				<p><b>14K</b></p>
			</span>
		</div>
		<div class="icon">
			<i class="far fa-heart"></i>
		</div>
	</div>
</body>
</html>
```
# កូដ CSS:
```javascript
body{
	margin: 0;
	padding: 0;
	background-color: #f1f1f1;
	display: flex;
	height: 100vh;
	justify-content: center;
	align-items: center;
	font-family: sans-serif;
}

.container {
	width: 900px;
	display: flex;
	background-color: #fff;
	box-shadow: 2px 2px 22px #3333;
	padding: 10px;
}

.container .image{
	width: 43%;
	margin-right: 2%;
}

.container .image img{
	width: 100%;
}

.container .content{
	width: 50%;
}

.container .content .title{
	font-size: 24px;
}

.container .content .paragraph{
	margin-bottom: 5px;
}

.container .content span{
	display: flex;
	align-items: center;
}

.container .content span i{
	font-size: 21px;
}

.container .icon{
	width: 5%;
}

.container .icon i{
	font-size: 30px;
	border: 1px solid #E74C3C;
	border-radius: 50%;
	padding: 8px;
	cursor: pointer;
}

@media (max-width: 910px){
	.container{
		flex-direction: column;
		width: 500px;
	}
	.container .image{
		width: 100%;
	}
	.container .content{
		width: 100%;
	}
	.container .icon{
		display: none;
	}
}

@media (max-width: 710px){
	.container{
		width: 300px;
	}
}
```
