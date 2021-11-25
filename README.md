
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta content="en-us" http-equiv="Content-Language" />
<meta content="text/html; charset=utf-8" http-equiv="Content-Type" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>主页</title>
</head>
<style>

* {
	padding: 0;
	margin: 0;
}


body {
	text-align: center;
	background-color: #ffffff;
}



img.smaller {
	width: 198px;
	height: 65px;
	max-width: 250px;
	animation: flipInX 4s;
	-webkit-animation: flipInX 4s
}




.logo {
	font-size: 2em;
	white-space: normal;
	word-wrap: break-word;
	text-decoration: none;
	color: #232323
}


#search_input {
	width: 90%;
	height: 40px;
	background-color: transparent;
	border: none;
	outline: 0;
	font-size: 18px;
	color: #426ab3;
	padding: 0 20px;
	border-radius: 50px
}


.search_part {
	margin-bottom: 30px;
	margin-top: 20px;
}


span {
	display: block;
	overflow: hidden;
	padding-left: 5px;
	vertical-align: middle;
}


.search_bar {
	box-shadow: 0 0 18px rgba(70,70,40,.255);
	-webkit-animation: fadeIn 2.5s;
	animation: fadeIn 2.5s;
	background-color: rgba(255,255,255,.100);
	border-radius: 50px;
	display: table;
	vertical-align: middle;
	width: 80%;
	height: 40px;
	max-width: 400px;
	margin: 10px auto;
}


#search_submit {
	outline: 0;
	height: 40px;
	float: right;
	color: #eee;
	font-size: 16px;
	font-weight: 700;
	border: none;
	background-color: transparent;
	padding: 0 13px 0 13px
}


#content {
	width: 100%;
	text-align: center;
	padding-top: 15px;
	padding-bottom: 15px;
}


.box {
	-webkit-animation: fadeInDown 1s;
	animation: fadeInDown 1s;
	position: relative;
	display: inline-block;
	width: 75px;
	border: 0;
}



.box a {
	width: 100%;
	height: 100%;
	position: absolute;
	left: 0;
	top: 0;
}


.url {
	color: #eee;
	height: 1.5em;
	line-height: 1.5em;
	width: 72px;
	font-size: 0.75em;
	white-space: nowrap;
	overflow: hidden;
	margin: auto;
	-webkit-border-top-right-radius: 5px;
	-webkit-border-bottom-right-radius: 5px;
	text-overflow: ellipsis;
	-o-text-overflow: ellipsis;
	-ms-text-overflow: ellipsis;
	padding-top: 3px;
	padding-bottom: 8px;
}

.icon {
	width: 3em;
	height: 3em;
	max-width: 72px;
}

@-webkit-keyframes flipInX {
	0% {
		-webkit-transform: perspective(400px) rotateX(90deg);
		transform: perspective(400px) rotateX(90deg);
		opacity: 0
	}

	40% {
		-webkit-transform: perspective(400px) rotateX(-10deg);
		transform: perspective(400px) rotateX(-10deg)
	}

	70% {
		-webkit-transform: perspective(400px) rotateX(10deg);
		transform: perspective(400px) rotateX(10deg)
	}

	100% {
		-webkit-transform: perspective(400px) rotateX(0);
		transform: perspective(400px) rotateX(0);
		opacity: 1
	}
}

@keyframes flipInX {
	0% {
		-webkit-transform: perspective(400px) rotateX(90deg);
		-ms-transform: perspective(400px) rotateX(90deg);
		transform: perspective(400px) rotateX(90deg);
		opacity: 0
	}

	40% {
		-webkit-transform: perspective(400px) rotateX(-10deg);
		-ms-transform: perspective(400px) rotateX(-10deg);
		transform: perspective(400px) rotateX(-10deg)
	}

	70% {
		-webkit-transform: perspective(400px) rotateX(10deg);
		-ms-transform: perspective(400px) rotateX(10deg);
		transform: perspective(400px) rotateX(10deg)
	}

	100% {
		-webkit-transform: perspective(400px) rotateX(0);
		-ms-transform: perspective(400px) rotateX(0);
		transform: perspective(400px) rotateX(0);
		opacity: 1
	}
}

@-webkit-keyframes fadeIn {
	0% {
		opacity: 0
	}

	100% {
		opacity: 1
	}
}

@keyframes fadeIn {
	0% {
		opacity: 0
	}

	100% {
		opacity: 1
	}
}

@-webkit-keyframes fadeInDown {
	0% {
		opacity: 0;
		-webkit-transform: translateY(-20px);
		transform: translateY(-20px)
	}

	100% {
		opacity: 1;
		-webkit-transform: translateY(0);
		transform: translateY(0)
	}
}

@keyframes fadeInDown {
	0% {
		opacity: 0;
		-webkit-transform: translateY(-20px);
		-ms-transform: translateY(-20px);
		transform: translateY(-20px)
	}

	100% {
		opacity: 1;
		-webkit-transform: translateY(0);
		-ms-transform: translateY(0);
		transform: translateY(0)
	}
}
</style>

<body>
<div id="content">
<br />
<div class="search_part">
<a class="logo" href="folder://">
<img class="smaller" src="logo/logo.gif"></img>
</a>
<br />
<form onsubmit="return search()" class="search_bar"
<span><input class="search" type="text" value="" autocomplete="off" id="search_input" ></span>
</form>
</div>
<br />

</div>

<script type="text/javascript">function search(){if(document.getElementById("search_input").value != ""){window.location.href = "https://www.baidu.com/s?word=" + document.getElementById("search_input").value;document.getElementById("search_input").value = "";}return false;}</script>

</body>
</html>
