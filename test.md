<html>
	<head>
		<title>Fallups | Frontend Framework</title>
		<link rel="shortcut icon" href="https://i.hizliresim.com/uu7GuX.png">
		<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css">
    	<link rel='stylesheet' href='https://unpkg.com/bulma@0.9.0/css/bulma.min.css'>
    	<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/overlayscrollbars/1.9.1/css/OverlayScrollbars.min.css'>
    	<link rel='stylesheet' href='https://kingsora.github.io/OverlayScrollbars/etc/os-theme-thin-dark.css'>	
		<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@300&display=swap" rel="stylesheet">
	</head>
	<body>
		<style>
			.mainFrame {
				width: 60%;
				height: 2900px;
				margin-left: auto;
  				margin-right: auto;
				margin-top: 50px;
				margin-bottom: 50px;
			}
			.grayTrap {
				width: 100%;
				height: 6px;
				border-radius: 25px;
				background-color: #646464;
			}
			.lightGrayTrap {
				width: 100%;
				height: 6px;
				border-radius: 25px;
				background-color: #C0C0C0;
				margin-top: 20px;
				margin-bottom: 20px;
			}
			* {
				font-family: 'Nunito', sans-serif;
			}
			.intro-npm {
				background: #242424;
				border-radius: 4px;
				color: #fff;
				display: flex;
				font-size: 15px;
				justify-content: space-between;
				line-height: 20px;
				padding: 15px 25px;
				position: relative;
			}
			.npmCopy:hover {
				color: orange;
				transition: 0.3s;
			}
			.npmCopy {
				color: white;
				transition: 0.3s;
			}
			pre {
				-webkit-overflow-scrolling: touch;
				background-color: #f5f5f5;
				color: #4a4a4a;
				font-size: .875em;
				overflow-x: auto;
				padding: 1.25rem 1.5rem;
				white-space: pre;
				word-wrap: normal;
			}
			code, pre {
				-moz-osx-font-smoothing: auto;
				-webkit-font-smoothing: auto;
				font-family: monospace;
			}
			.tooltip {
				position: relative;
				display: inline-block;
				border-bottom: 1px dotted black;
			}
			.tooltip .tooltiptext {
				visibility: hidden;
				width: 220px;
				background-color: black;
				color: #fff;
				text-align: center;
				padding: 5px 0;
				border-radius: 6px;
				position: absolute;
				z-index: 1;
			}
			.tooltip:hover .tooltiptext {
				visibility: visible;
			}
		</style>
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
		<script>
			function kopyala(element) {
			  var $temp = $("<input>");
			  $("body").append($temp);
			  $temp.val($(element).text()).select();
			  document.execCommand("copy");
			  alert("Kopyalandı: " + $temp.val($(element).text())[0].value)
			  $temp.remove();
			}
		</script>
		<script src="https://cdn.jsdelivr.net/npm/fallups@0.0.2/js/fallups.js"></script>
		<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/fallups@0.0.2/css/fallups.css">
		<div class="mainFrame">
			<center>
				<img src="https://i.ibb.co/ngxGy67/fallups.png" style="width: 40%;">
			</center>

			<div class="grayTrap"></div>
			
			<center>
				<h1 style="font-size: 40px; margin-left: 30px; margin-top: 20px;"><b>v</b>0.0.2</h1>
			</center>
			
			<div class="lightGrayTrap"></div>

			<h1 style="font-size: 40px; margin-left: 30px; margin-top: 20px;">Hakkında</h1>
			<h3 style="font-size: 25px; margin-left: 30px;">Fallups bir frontend çatısıdır, hazır CSS'ler classlar ve scriptler içerir. <br>Kurulum için sadece 2 satır kod yeterlidir, kurulum aşağıda detaylı bir şekilde anlatılmıştır. Örnek kullanımlar sayfanın altında yer almaktadır.</h3>

			<div class="lightGrayTrap"></div>

			<h1 style="font-size: 40px; margin-left: 30px; margin-top: 20px;">Kurulum</h1>
			<h3 style="font-size: 25px; margin-left: 30px;">Kurulum için aşağıdaki 2 kodu HTML dosyanıza atmanız yeterlidir.</h3>
			
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">CSS <b style="font-size: 15px;">(Kopyalamak için kodun üstüne tıklayın!)</b></h4>
			<pre onclick="kopyala('#kopyala1')" id="npm" class="intro-npm"><code id="kopyala1">&lt;script src="https://cdn.jsdelivr.net/npm/fallups@latest/js/fallups.js">&lt;/script></code></pre>
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">JS <b style="font-size: 15px;">(Kopyalamak için kodun üstüne tıklayın!)</b></h4>
			<pre onclick="kopyala('#kopyala2')" id="npm" style="margin-bottom: 10px;" class="intro-npm"><code id="kopyala2">&lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/fallups@0.0.2/css/fallups.css"></code></pre>
			
			<div class="lightGrayTrap"></div>
			
			<h1 style="font-size: 40px; margin-left: 30px; margin-top: 20px;">Dokümanlar</h1>
			<h3 style="font-size: 25px; margin-left: 30px;">Fallups'un nasıl kullanılacağı hakkında örnekler aşağıda yer almaktadır.</h3>
			
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Düğme Oluşturma</h4>
			<pre id="npm" class="intro-npm"><code id="kopyala3">&lt;button href="#" class="button">Tıkla!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala3')">kopyala</a></pre>
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Çıktı</h4>
			<button href="#" class="button">Tıkla!</button>
			<br><br>
			
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Düğme Renklendirme</h4>
			<pre id="npm" class="intro-npm"><code id="kopyala4">&lt;button href="#" class="button button-error">Error!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala4')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala5">&lt;button href="#" class="button button-warn">Warn!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala5')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala6">&lt;button href="#" class="button button-info">Info!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala6')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala7">&lt;button href="#" class="button button-ok">Ok!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala7')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala8">&lt;button href="#" class="button button-dark">Dark!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala8')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala9">&lt;button href="#" class="button button-light">Light!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala9')">kopyala</a></pre>
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Çıktı</h4>
			<button href="#" class="button button-error">Error!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-warn">Warn!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-info">Info!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-ok">Ok!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-dark">Dark!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-light">Light!</button>
			<br><br>
			
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Düğmeleri Dışhatlı Yapma</h4>
			<pre id="npm" class="intro-npm"><code id="kopyala10">&lt;button href="#" class="button button-outline-error">Error!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala10')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala11">&lt;button href="#" class="button button-outline-warn">Warn!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala11')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala12">&lt;button href="#" class="button button-outline-info">Info!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala12')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala13">&lt;button href="#" class="button button-outline-ok">Ok!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala13')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala14">&lt;button href="#" class="button button-outline-dark">Dark!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala14')">kopyala</a></pre>
			<pre id="npm" style="margin-top: 10px;" class="intro-npm"><code id="kopyala15">&lt;button href="#" class="button button-outline-light">Light!&lt;/button></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala15')">kopyala</a></pre>
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Çıktı</h4>
			<button href="#" class="button button-outline-error">Error!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-outline-warn">Warn!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-outline-info">Info!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-outline-ok">Ok!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-outline-dark">Dark!</button>&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160&#160
			<button href="#" class="button button-outline-light">Light!</button>
			<br><br>
			
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Bildirim Düğmesi</h4>
			<pre id="npm" class="intro-npm"><code id="kopyala16">&lt;button onclick="fallups.notification();" href="#" class="button button-outline-dark">Tıkla bana ve mesajı gör!&lt;/button><br>&lt;div id="notification">Merhaba sayın okuyucu!&lt;/div></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala16')"><br>kopyala</a></pre>
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Çıktı</h4>
			<button onclick="fallups.notification();" href="#" class="button button-outline-dark">Tıkla bana ve mesajı gör!</button><div id="notification">Merhaba sayın okuyucu!</div>
			<br><br>
			
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Header (Navigasyon Çubuğu)</h4>
			<pre id="npm" class="intro-npm"><code id="kopyala17">&lt;fallupsHeader class="header-dark"><br>  &lt;a href="/" style="color: white;" class="header-item">TEST&lt;/a><br>  &lt;a href="/" style="color: white;" class="header-item-right">TEST&lt;/a><br>  &lt;a href="/" style="color: white;" class="header-item-right">TEST&lt;/a><br>&lt;/fallupsHeader></code><a id="npmCopy" class="intro-npm-copy npmCopy" onclick="kopyala('#kopyala17')"><br><br>kopyala</a></pre>
			<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Çıktı <b style="font-size: 15px;">(Header çıktısını burada gösteremem.)</b></h4>
			<br><br>
			
			<div class="lightGrayTrap"></div>
			
			<h1 style="font-size: 40px; margin-left: 30px; margin-top: 20px;">Geliştirici</h1>
			<center>
				<div class="tooltip" style="font-size: 25px; margin-top: 20px; margin-left: 30px;">
					Swôth#9990
					<center>
						<span style="font-size: 15px; margin-top: -70px; margin-left: -100px;" class="tooltiptext"><a href="https://github.com/rennia" style="color: white;">Member of teamRennia</a></span>
					</center>
				</div>
				
			</center>
			
			<div class="lightGrayTrap"></div>
			
			<center>
				<h4 style="font-size: 20px; margin-top: 15px; margin-left: 20px;">Copyright © 2020 Swôth | Licensed under Apache-2.0</h4>
			</center>
		</div>
	</body>
</html>
