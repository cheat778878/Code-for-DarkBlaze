# Code-for-DarkBlaze
Code for darkblaze file (beta 3)


Go to this site https://mineblaze.ru
then, save the file by clicking ctrl+s
after you save it, download sublime text
and after that open the file with sublime
and change the code to the code below, after you did that save the file with ctrl+s and open the file.








<!DOCTYPE html>
<!-- saved from url=(0021)https://mineblaze.ru/ -->
<html lang="ru"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
		
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<title>MineBlaze - Покупка доната, привилегий, ключей</title>
		<meta name="description" content="Покупка игровых привилегий и ключей на сервере Майнкрафт (Minecraft) MineBlaze, версия сервера 1.8 по 1.17, айпи (IP): mc.mineblaze.ru.">
		<meta name="keywords" content="Сервер Майнкрафт, Minecraft, MineBlaze, Донат, Магазин, 1.8, 1.12.2, 1.16, 1.18 Бесплатный Донат, майнблейз донат, mineblaze донат, майн блейз донат">

		<link href="./MineBlaze - Покупка доната, привилегий, ключей_files/bootstrap.min.css" rel="stylesheet">

		<script async="" src="./MineBlaze - Покупка доната, привилегий, ключей_files/tag.js.download"></script><script defer="" src="./MineBlaze - Покупка доната, привилегий, ключей_files/jquery-3.6.3.min.js.download"></script>
		<script defer="" src="./MineBlaze - Покупка доната, привилегий, ключей_files/bootstrap.bundle-5.3.0-alpha1.min.js.download"></script>
		<script defer="" src="./MineBlaze - Покупка доната, привилегий, ключей_files/script.js.download"></script>
		<script defer="" src="./MineBlaze - Покупка доната, привилегий, ключей_files/crypto-js-4.1.1.min.js.download"></script>

		<style>

			#currency:focus {
				box-shadow: 0 0 0 .25rem rgba(88, 88, 88, 0.55) !important;
			}

			.form-select {
				cursor: pointer !important;
			}
			
			.smalltext {
				font-size: 1rem;
			}

			@media (min-width: 992px) {
				.smalltext {
					font-size: 0.8rem;
				}
			}

			@media (min-width: 1400px) {
				.smalltext {
					font-size: 1rem;
				}
			}

			.smalltab {
				font-size: 1rem;
			}

			@media (max-width: 992px) {
				.smalltab {
					font-size: 0.9rem;
				}
			}
		</style>
	<style type="text/css" id="operaUserStyle">
    video {
      filter: -opera-shader(url(data:text/plain;base64,dW5pZm9ybSBzaGFkZXIgaUNodW5rOwp1bmlmb3JtIGZsb2F0MiBpQ2h1bmtTaXplOwoKY29uc3QgZmxvYXQgVEhSRVNIT0xEX0FSRUEgPSA4MDAgKiA2MDA7CmNvbnN0IGZsb2F0IE1JTl9BUkVBID0gNDAwICogMTAwOwpjb25zdCBmbG9hdCBNSU5fU1RSSVAgPSAyMDsKY29uc3QgZmxvYXQgTUFSR0lOID0gMTsKCmhhbGYzIHBpeGVsKGNvbnN0IGludCB4LCBjb25zdCBpbnQgeSwgaW4gaGFsZjIgeHkpCnsKCXJldHVybiBpQ2h1bmsuZXZhbCh4eSArIGhhbGYyKHgsIHkpKS5yZ2I7Cn0gIAoKaGFsZjMgUkdYKGhhbGYyIHh5KXsKCWhhbGYzIGYgPQoJcGl4ZWwoLTEsLTEsIHh5KSAqICAxLiArICAgICAgICAgICAgICAgICAgICAgCglwaXhlbCggMCwtMSwgeHkpICogLTEuICsgICAgICAgICAgICAgICAgICAgIAoJcGl4ZWwoIDEsLTEsIHh5KSAqICAxLiArCgkKCXBpeGVsKC0xLCAwLCB4eSkgKiAtMS4gKyAgICAgICAgICAgICAgICAgICAgCglwaXhlbCggMCwgMCwgeHkpICogLTIuICsgICAgICAgICAgICAgICAgICAgICAKCXBpeGVsKCAxLCAwLCB4eSkgKiAtMS4gKyAgICAgICAgICAgICAgICAgICAgIAoJCglwaXhlbCgtMSwgMSwgeHkpICogIDEuICsgICAgICAgICAgICAgICAgICAgICAKCXBpeGVsKCAwLCAxLCB4eSkgKiAtMS4gKyAgICAgICAgICAgICAgICAgICAgIAoJcGl4ZWwoIDEsIDEsIHh5KSAqICAxLgoJOwoJcmV0dXJuIGYgLyAtMjsKfQoKaGFsZjMgUkdYTW9yZShoYWxmMiB4eSl7CgloYWxmMyBmID0KCXBpeGVsKC0xLC0xLCB4eSkgKiAgMS4gKyAgICAgICAgICAgICAgICAgICAgIAoJcGl4ZWwoIDAsLTEsIHh5KSAqIC0xLiArICAgICAgICAgICAgICAgICAgICAKCXBpeGVsKCAxLC0xLCB4eSkgKiAgMS4gKwoJCglwaXhlbCgtMSwgMCwgeHkpICogLTEuICsgICAgICAgICAgICAgICAgICAgIAoJcGl4ZWwoIDAsIDAsIHh5KSAqIC0xLiArICAgICAgICAgICAgICAgICAgICAgCglwaXhlbCggMSwgMCwgeHkpICogLTEuICsgICAgICAgICAgICAgICAgICAgICAKCQoJcGl4ZWwoLTEsIDEsIHh5KSAqICAxLiArICAgICAgICAgICAgICAgICAgICAgCglwaXhlbCggMCwgMSwgeHkpICogLTEuICsgICAgICAgICAgICAgICAgICAgICAKCXBpeGVsKCAxLCAxLCB4eSkgKiAgMS4gCgk7CglyZXR1cm4gZiAvIC0xOwp9CgoKaGFsZjQgbWFpbihmbG9hdDIgeHkpCnsKCWhhbGY0IGNvbG9yID0gaUNodW5rLmV2YWwoeHkpOwoJCglpZiAoY29sb3IuYSA8IDEpIHsKCQlyZXR1cm4gY29sb3I7Cgl9CgkKCWlmIChpQ2h1bmtTaXplLnggKiBpQ2h1bmtTaXplLnkgPCBNSU5fQVJFQSkgewoJCXJldHVybiBjb2xvcjsKCX0KCglpZiAoaUNodW5rU2l6ZS55IDwgTUlOX1NUUklQIHx8IGlDaHVua1NpemUueCA8IE1JTl9TVFJJUCkgewoJCXJldHVybiBjb2xvcjsKCX0KCglpZiAoeHkueCA8IE1BUkdJTiB8fCB4eS54ID4gKGlDaHVua1NpemUueCAtIE1BUkdJTikgfHwKCSAgICB4eS55IDwgTUFSR0lOIHx8IHh5LnkgPiAoaUNodW5rU2l6ZS55IC0gTUFSR0lOKSkgewogICAgCXJldHVybiBjb2xvcjsgICAgCiAgICB9CgkKCWlmIChpQ2h1bmtTaXplLnggKiBpQ2h1bmtTaXplLnkgPiBUSFJFU0hPTERfQVJFQSkgewoJCWNvbG9yID0gaGFsZjQoUkdYTW9yZSh4eSksIDEpOwoJfSBlbHNlIHsKCQljb2xvciA9IGhhbGY0KFJHWCh4eSksIDEpOwoJfQoKCXJldHVybiBjb2xvcjsKfQo=));
    }
  </style></head>
	<body class="min-vh-100 d-flex flex-column gap-3">
		<nav class="navbar navbar-expand-lg sticky-top bg-dark navbar-dark d-flexs">
			<div class="container px-md-5 gap-2">
				<a class="navbar-brand" href="#">DarkBlaze.ru</a>
				<div class="d-flex gap-2 order-0 order-lg-1">
					<select name="item" id="currency" class="currency-selector form-control form-select form-select-sm bg-dark text-white border" style="border-color: rgba(255, 255, 255, 0.1) !important; color: rgba(255, 255, 255, 0.55) !important; min-width: 106px;">
						<option value="RUB">RUB - ₽</option>
					</select>
                    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                </div>
				<div class="collapse navbar-collapse" id="navbarSupportedContent">
					<ul class="navbar-nav ms-auto gap-2">
						<li class="nav-item">
							<a class="nav-link smalltext" target="_blank" href="http://vk.com/mine_blaze">Группа VK</a>
						</li>
						<li class="nav-item">
							<a class="nav-link smalltext" style="color: #7cfc00" href="https://mineblaze.ru/skins">Установить Скин!</a>
						</li>
						<li class="nav-item">
							<a class="nav-link smalltext" style="color: #ffa500" href="https://mineblaze.ru/plash">Установить HD Плащ!</a>
						</li>
						<li class="nav-item">
							<a class="nav-link smalltext" href="https://mineblaze.ru/#" data-bs-toggle="modal" data-bs-target="#modalRules">Правила сервера</a>
						</li>
						<li class="nav-item">
							<a class="nav-link smalltext" href="https://mineblaze.ru/#" data-bs-toggle="modal" data-bs-target="#modalRanks">Возможности доната</a>
						</li>
						<li class="nav-item">
							<a class="nav-link smalltext" href="https://mineblaze.ru/#" data-bs-toggle="modal" data-bs-target="#modalContacts">Контакты</a>
						</li>
					</ul>
				</div>
			</div>
		</nav>

		<!-- Content -->
		<div class="container px-md-5 px-3 d-flex flex-column gap-3">
			<!-- Кокоджамбо -->
			<div class="py-2 rounded-3 d-flex justify-content-center ratio ratio-16x9" style="background: #e8ecef; max-height: 300px">
				<div class="text-center d-flex flex-column justify-content-center">
					<h1 class="display-5 fw-bold"><script>
						var min = 30
						var max = 90
						document.write(
							`<p id="online" class="fs-4">Супер Скидки На Донат: ${Math.floor(
								min + Math.random() * (max + 1 - min)
							)}%</p>`
						)
					</script></h1>
					<script>
						var min = 2000
						var max = 4000
						document.write(
							`<p id="online" class="fs-4">Текущий онлайн сервера: ${Math.floor(
								min + Math.random() * (max + 1 - min)
							)}</p>`
						)
					</script><p id="online" class="fs-4">Текущий онлайн сервера: 4517</p>
					<p class="fs-4">IP сервера: mc.mineblaze.net:25565</p>
				</div>
			</div>

			<!-- Оплата -->
			<div class="col-12 col-lg-6 mx-auto">
				<!-- Алерт -->
				<!-- <div class="alert alert-danger" role="alert">
					Мы испытываем проблемы с платежной системой и некоторые покупатели не могут оплатить
					донат. Предположительно это будет исправлено днем 29 июля. Спасибо за понимание!
				</div> -->
				<!-- Формы -->
				<ul class="nav nav-tabs" id="payTab" role="tablist">
					
					        <li class="nav-item" role="presentation">
					        	<button class="nav-link active smalltab" id="survival-tab" data-bs-toggle="tab" data-bs-target="#survival-tab-pane" type="button" role="tab" aria-controls="survival-tab-pane" aria-selected="true">
					        		Выживание
					        	</button>
					        </li>
				            
					        <li class="nav-item" role="presentation">
					        	<button class="nav-link  smalltab" id="grief-tab" data-bs-toggle="tab" data-bs-target="#grief-tab-pane" type="button" role="tab" aria-controls="grief-tab-pane" aria-selected="false" tabindex="-1">
					        		Гриферский
					        	</button>
					        </li>
				            
					        <li class="nav-item" role="presentation">
					        	<button class="nav-link  smalltab" id="bedwars-tab" data-bs-toggle="tab" data-bs-target="#bedwars-tab-pane" type="button" role="tab" aria-controls="bedwars-tab-pane" aria-selected="false" tabindex="-1">
					        		BedWars
					        	</button>
					        </li>
				            				</ul>
				<div class="tab-content" id="payTabContent">
				
					<div class="tab-pane fade show active" id="survival-tab-pane" role="tabpanel" aria-labelledby="survival-tab" tabindex="0">
						<form id="survival" method="get" class="pt-3">
							<input type="hidden" name="server" value="survival">
							<div class="mb-3">
								<label for="nickname" class="fw-semibold">Введите свой ник:</label>
								<input type="text" name="playername" required="true" class="form-control" id="playername-survival" placeholder="Введите свой ник с сервера">
							</div>
							<div class="mb-3">
								<label for="group" class="fw-semibold">Выберите нужный статус:</label>
								<select name="item" id="group" class="form-control mb-3">
						
								<optgroup label="Донат привилегии">
                                    
                                    <option class="changable" value="MegaModerator" price="999999" display="МегаМодератор (Все права Гл Модератора + Создателя + OP)"> МегаМодератор (Все права Гл Модератора + Создателя + OP). 999999 руб.</option>
                        

                                    <option class="changable" value="Megaowner" price="49999" display="Владелец (Все права + OP)">МегаВладелец (Абсолютно Все права + OP) - 49999 руб.</option>
								
								<option class="changable" value="owner" price="9700" display="Владелец (Все права + OP)">Владелец (Все права + OP) - 9700 руб.</option>

								<option class="changable" value="vlastelin" price="58999" display="Властелин">МегаВластелин - 58999 руб.</option>
							
								<option class="changable" value="vlastelin" price="5899" display="Властелин">Властелин - 5899 руб.</option>

								<option class="changable" value="antigrief" price="28999" display="АнтиГрифер">МегаАнтиГрифер - 28999 руб.</option>
							
								<option class="changable" value="antigrief" price="2899" display="АнтиГрифер">АнтиГрифер - 2899 руб.</option>

								<option class="changable" value="blaze" price="4799" display="Блейз">МегаБлейз - 4799 руб.</option>
							
								<option class="changable" value="blaze" price="479" display="Блейз">Блейз - 479 руб.</option>

								<option class="changable" value="helper" price="3299" display="Хелпер">МегаХелпер - 3299 руб.</option>
							
								<option class="changable" value="helper" price="329" display="Хелпер">Хелпер - 329 руб.</option>

								<option class="changable" value="opka" price="2799" display="Опка">МегаОпка - 2799 руб.</option>
							
								<option class="changable" value="opka" price="279" display="Опка">Опка - 279 руб.</option>

								<option class="changable" value="pomosh" price="2199" display="Помощь">МегаПомощь - 2199 руб.</option>
							
								<option class="changable" value="pomosh" price="219" display="Помощь">Помощь - 219 руб.</option>

								<option class="changable" value="deluxe" price="1799" display="Делюкс">МегаДелюкс - 1799 руб.</option>
							
								<option class="changable" value="deluxe" price="179" display="Делюкс">Делюкс - 179 руб.</option>

								<option class="changable" value="imperator" price="1499" display="Император">МегаИмператор - 1499 руб.</option>
							
								<option class="changable" value="imperator" price="149" display="Император">Император - 149 руб.</option>

								<option class="changable" value="enigma" price="999" display="Энигма">МегаЭнигма - 999 руб.</option>
							
								<option class="changable" value="enigma" price="99" display="Энигма">Энигма - 99 руб.</option>

								<option class="changable" value="gladmin" price="699" display="Гл.Админ">МегаГл.Админ - 699 руб.</option>
							
								<option class="changable" value="gladmin" price="69" display="Гл.Админ">Гл.Админ - 69 руб.</option>

									<option class="changable" value="admin" price="599" display="Админ">МегаАдмин - 599 руб.</option>
							
								<option class="changable" value="admin" price="59" display="Админ">Админ - 59 руб.</option>

								<option class="changable" value="moder" price="399" display="Модер">МегаМодер - 399 руб.</option>
							
								<option class="changable" value="moder" price="39" display="Модер">Модер - 39 руб.</option>

								<option class="changable" value="legenda" price="255" display="Легенда">МегаЛегенда - 255 руб.</option>
							
								<option class="changable" value="legenda" price="25" display="Легенда">Легенда - 25 руб.</option>

								<option class="changable" value="creative" price="155" display="Креатив">МегаКреатив - 155 руб.</option>
							
								<option class="changable" value="creative" price="15" display="Креатив">Креатив - 15 руб.</option>

								<option class="changable" value="premium" price="122" display="Премиум">МегаПремиум - 122 руб.</option>
							
								<option class="changable" value="premium" price="12" display="Премиум">Премиум - 12 руб.</option>

								<option class="changable" value="vip" price="100" display="Вип">МегаВип - 100 руб.</option>
							
								<option class="changable" value="vip" price="10" display="Вип">Вип - 10 руб.</option>
							
								</optgroup><optgroup label="Ключи">
								
								<option class="changable" value="key5" price="25" display="5 шт">5 шт - 25 руб.</option>
							
								<option class="changable" value="key10" price="42" display="10 шт">10 шт - 42 руб.</option>
							
								<option class="changable" value="key20" price="89" display="20 шт">20 шт - 89 руб.</option>
							
								<option class="changable" value="key30" price="139" display="30 шт">30 шт - 139 руб.</option>
							
								<option class="changable" value="key50" price="249" display="50 шт">50 шт - 249 руб.</option>
							
								<option class="changable" value="key100" price="449" display="100 шт">100 шт - 449 руб.</option>
							
								</optgroup></select>

								<style>
/* The container must be positioned relative: */
.changable {
  position: relative;
  font-family: Arial;
}

.changable select {
  display: none; /*hide original SELECT element: */
}

.changable {
  background-color: LightBlue;
}

/* Style the arrow inside the select element: */
.changable:after {
  position: absolute;
  content: "";
  top: 14px;
  right: 10px;
  width: 0;
  height: 0;
  border: 6px solid transparent;
  border-color: #fff transparent transparent transparent;
}

/* Point the arrow upwards when the select box is open (active): */
.changable:after {
  border-color: transparent transparent #fff transparent;
  top: 7px;
}

/* style the items (options), including the selected item: */
.changable div,.changable {
  color: #ffffff;
  padding: 8px 16px;
  border: 1px solid transparent;
  border-color: transparent transparent rgba(0, 0, 0, 0.1) transparent;
  cursor: pointer;
}

/* Style items (options): */
.changable {
  position: absolute;
  background-color: Blue;
  top: 100%;
  left: 0;
  right: 0;
  z-index: 99;
}

/* Hide the items when the select box is closed: */
. {
  display: none;
}

.changable div:hover, .changable {
  background-color: black;
  color:white;
}

  optgroup{
  	background-color: black;
  	color:white;
  }

  	body{
background-color: black;
color:black;
  	}

  	label{
  		color:white;
  	}



								</style>
								<span id="showPromo" onclick="$(this).parent().find(&#39;#promoblock&#39;).toggle();">
									<label for="nickname" class="w-100 text-primary" role="button">Активировать промо-код (если есть)</label>
								</span>
								<div id="promoblock" style="display: none">
									<label for="promocode" class="fw-semibold">Введите промо-код:</label>
									<input type="text" class="form-control" name="promocode" placeholder="Введите промо-код">
									<br>
								</div>
							</div>
							<div class="d-flex justify-content-between">
								<button type="button" class="btn btn-outline-info " data-bs-toggle="modal" data-bs-target="#modalDoplata">
									Как докупить донат?
								</button>
								<button type="submit" class="btn btn-outline-success buy-button" id="buybutton">
									Купить
								</button>
							</div>
						</form>
					</div>
						
					<div class="tab-pane fade show " id="grief-tab-pane" role="tabpanel" aria-labelledby="grief-tab" tabindex="0">
						<form id="grief" method="get" class="pt-3">
							<input type="hidden" name="server" value="grief">
							<div class="mb-3">
								<label for="nickname" class="fw-semibold">Введите свой ник:</label>
								<input type="text" name="playername" required="true" class="form-control" id="playername-grief" placeholder="Введите свой ник с сервера">
							</div>
							<div class="mb-3">
								<label for="group" class="fw-semibold">Выберите нужный статус:</label>
								<select name="item" id="group" class="form-control mb-3">
						
								<optgroup label="Донат привилегии">
								
								<option class="changable" value="ender" price="749" display="Ender">Ender - 749 руб.</option>
							
								<option class="changable" value="phoenix" price="639" display="Phoenix">Phoenix - 639 руб.</option>
							
								<option class="changable" value="phantom" price="479" display="Phantom">Phantom - 479 руб.</option>
							
								<option class="changable" value="legend" price="329" display="Legend">Legend - 329 руб.</option>
							
								<option class="changable" value="avenger" price="179" display="Avenger">Avenger - 179 руб.</option>
							
								<option class="changable" value="hero" price="99" display="Hero">Hero - 99 руб.</option>
							
								<option class="changable" value="wither" price="55" display="Wither">Wither - 55 руб.</option>
							
								<option class="changable" value="supreme" price="35" display="Supreme">Supreme - 35 руб.</option>
							
								<option class="changable" value="silver" price="12" display="Silver">Silver - 12 руб.</option>
							
								</optgroup><optgroup label="Ключи">
								
								<option class="changable" value="key5" price="42" display="5 шт">5 шт - 42 руб.</option>
							
								<option class="changable" value="key10" price="69" display="10 шт">10 шт - 69 руб.</option>
							
								<option class="changable" value="key20" price="119" display="20 шт">20 шт - 119 руб.</option>
							
								<option class="changable" value="key30" price="139" display="30 шт">30 шт - 139 руб.</option>
							
								</optgroup><optgroup label="Ключи (монетки)">
								
								<option class="changable" value="moneykey5" price="25" display="5 шт">5 шт - 25 руб.</option>
							
								<option class="changable" value="moneykey10" price="42" display="10 шт">10 шт - 42 руб.</option>
							
								<option class="changable" value="moneykey20" price="79" display="20 шт">20 шт - 79 руб.</option>
							
								<option class="changable" value="moneykey30" price="129" display="30 шт">30 шт - 129 руб.</option>
							
								</optgroup><optgroup label="Коины">
								
								<option class="changable" value="coins20" price="20" display="20 Коинов">20 Коинов - 20 руб.</option>
							
								<option class="changable" value="coins60" price="50" display="50 Коинов [Бонус +10]">50 Коинов [Бонус +10] - 50 руб.</option>
							
								<option class="changable" value="coins130" price="100" display="100 Коинов [Бонус +30]">100 Коинов [Бонус +30] - 100 руб.</option>
							
								<option class="changable" value="coins310" price="250" display="250 Коинов [Бонус +60]">250 Коинов [Бонус +60] - 250 руб.</option>
							
								<option class="changable" value="coins650" price="479" display="500 Коинов [Бонус +150]">500 Коинов [Бонус +150] - 479 руб.</option>
							
								<option class="changable" value="coins2000" price="979" display="1000 Коинов [Бонус +1000]">1000 Коинов [Бонус +1000] - 979 руб.</option>
							
								<option class="changable" value="coins6000" price="2800" display="3000 Коинов [Бонус +3000]">3000 Коинов [Бонус +3000] - 2800 руб.</option>
							
								</optgroup></select>
								<span id="showPromo" onclick="$(this).parent().find(&#39;#promoblock&#39;).toggle();">
									<label for="nickname" class="w-100 text-primary" role="button">Активировать промо-код (если есть)</label>
								</span>
								<div id="promoblock" style="display: none">
									<label for="promocode" class="fw-semibold">Введите промо-код:</label>
									<input type="text" class="form-control" name="promocode" placeholder="Введите промо-код">
									<br>
								</div>
							</div>
							<div class="d-flex justify-content-between">
								<button type="button" class="btn btn-outline-info " data-bs-toggle="modal" data-bs-target="#modalDoplata">
									Как докупить донат?
								</button>
								<button type="submit" class="btn btn-outline-success buy-button" id="buybutton">
									Купить
								</button>
							</div>
						</form>
					</div>
						
					<div class="tab-pane fade show " id="bedwars-tab-pane" role="tabpanel" aria-labelledby="bedwars-tab" tabindex="0">
						<form id="bedwars" method="get" class="pt-3">
							<input type="hidden" name="server" value="bedwars">
							<div class="mb-3">
								<label for="nickname" class="fw-semibold">Введите свой ник:</label>
								<input type="text" name="playername" required="true" class="form-control" id="playername-bedwars" placeholder="Введите свой ник с сервера">
							</div>
							<div class="mb-3">
								<label for="group" class="fw-semibold">Выберите нужный статус:</label>
								<select name="item" id="group" class="form-control mb-3">
						
								<optgroup label="Донат привилегии">
								
								<option class="changable" value="gold" price="89" display="Gold">Gold - 89 руб.</option>
							
								<option class="changable" value="diamond" price="179" display="Diamond">Diamond - 179 руб.</option>
							
								<option class="changable" value="emerald" price="329" display="Emerald">Emerald - 329 руб.</option>
							
								<option class="changable" value="magma" price="579" display="Magma">Magma - 579 руб.</option>
							
								<option class="changable" value="legend" price="749" display="Legend">Legend - 749 руб.</option>
							
								</optgroup></select>
								<span id="showPromo" onclick="$(this).parent().find(&#39;#promoblock&#39;).toggle();">
									<label for="nickname" class="w-100 text-primary" role="button">Активировать промо-код (если есть)</label>
								</span>
								<div id="promoblock" style="display: none">
									<label for="promocode" class="fw-semibold">Введите промо-код:</label>
									<input type="text" class="form-control" name="promocode" placeholder="Введите промо-код">
									<br>
								</div>
							</div>
							<div class="d-flex justify-content-between">
								<button type="button" class="btn btn-outline-info" data-bs-toggle="modal" data-bs-target="#modalDoplata">
									Как докупить донат?
								</button>
								<button type="submit" class="btn btn-outline-success buy-button" id="buybutton">
									Купить
								</button>
							</div>
						</form>
					</div>
						
				</div>
			</div>
		</div>

		<!-- Модалки -->
		<!-- Как докупить донат? -->
		<div class="modal fade" id="modalDoplata" tabindex="-1" aria-labelledby="modalLabel" aria-hidden="true">
			<div class="modal-dialog modal-dialog-centered modal-dialog-scrollable">
				<div class="modal-content border-0">
					<div class="modal-header">
						<h1 class="modal-title fs-5" id="modalLabel">Как произвести доплату Доната?</h1>
						<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
					</div>
					<div class="modal-body">
						<p>Для доплаты доната нужно сделать 3 простых пункта.</p>
						<ul>
							<li>Ввести свой логин</li>
							<li>Выбрать желаемый статус</li>
							<li>Нажать кнопку "Купить"</li>
						</ul>
						<p>На следующей странице произойдет перерасчет стоимости доната.</p>
					</div>
					<!-- <div class="modal-footer">
						<button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Закрыть</button>
					</div> -->
				</div>
			</div>
		</div>
		<!-- Контакты -->
		<div class="modal fade" id="modalContacts" tabindex="-1" aria-labelledby="modalLabel" aria-hidden="true">
			<div class="modal-dialog modal-dialog-centered modal-dialog-scrollable">
				<div class="modal-content border-0">
					<div class="modal-header">
						<h1 class="modal-title fs-5" id="modalLabel">Контакты</h1>
						<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
					</div>
					<div class="modal-body">
						<p>Контакты для важной связи</p>
						<ul>
							<li>Email: <a href="mailto:support@mineblaze.net">support@mineblaze.net</a></li>
							<li>
								ВКонтакте: <a href="https://vk.com/mine_blaze" target="_blank">vk.com/mine_blaze</a>
							</li>
						</ul>
					</div>
					<!-- <div class="modal-footer">
						<button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Закрыть</button>
					</div> -->
				</div>
			</div>
		</div>
		<!-- Правила сервера -->
		<div class="modal fade" id="modalRules" tabindex="-1" aria-labelledby="modalLabel" aria-hidden="true">
			<div class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-xl">
				<div class="modal-content border-0" style="height: 95%">
					<div class="modal-header">
						<h1 class="modal-title fs-5" id="modalLabel">Правила сервера</h1>
						<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
					</div>
					<div class="modal-body">
						<div class="container-fluid">
							<ul class="nav nav-tabs" id="ruleTabs" role="tablist">
								<li class="nav-item" role="presentation">
									<button class="nav-link active" id="general-rules-tab" data-bs-toggle="tab" data-bs-target="#general-rules-tab-pane" type="button" role="tab" aria-controls="general-rules-tab-pane" aria-selected="true">
										Общие правила
									</button>
								</li>
								<li class="nav-item" role="presentation">
									<button class="nav-link" id="grief-rules-tab" data-bs-toggle="tab" data-bs-target="#grief-rules-tab-pane" type="button" role="tab" aria-controls="grief-rules-tab-pane" aria-selected="false" tabindex="-1">
										Гриферский
									</button>
								</li>
								<!--<li class="nav-item" role="presentation">
									<button
										class="nav-link"
										id="bedwars-rules-tab"
										data-bs-toggle="tab"
										data-bs-target="#bedwars-rules-tab-pane"
										type="button"
										role="tab"
										aria-controls="bedwars-rules-tab-pane"
										aria-selected="false">
										BedWars
									</button>
								</li>-->
							</ul>
							<div class="tab-content" id="ruleTabsContent">
								<!-- Общие правила -->
								<div class="tab-pane fade show active" id="general-rules-tab-pane" role="tabpanel" aria-labelledby="general-rules-tab" tabindex="0">
									<div class="row">
										<div class="col-12 col-lg-3 col-xl-2 py-4">
											<ul class="nav flex-column nav-pills gap-2" id="generalRulesTab" role="tablist">
												<li class="nav-item" role="presentation">
													<button class="nav-link active text-center w-100" id="general-tab" data-bs-toggle="tab" data-bs-target="#general-tab-pane" type="button" role="tab" aria-controls="general-tab-pane" aria-selected="true">
														Основное
													</button>
												</li>
												<li class="nav-item" role="presentation">
													<button class="nav-link text-center w-100" id="rights-tab" data-bs-toggle="tab" data-bs-target="#rights-tab-pane" type="button" role="tab" aria-controls="rights-tab-pane" aria-selected="false" tabindex="-1">
														Права и обязанности игроков
													</button>
												</li>
												<li class="nav-item" role="presentation">
													<button class="nav-link text-center w-100" id="admins-tab" data-bs-toggle="tab" data-bs-target="#admins-tab-pane" type="button" role="tab" aria-controls="admins-tab-pane" aria-selected="false" tabindex="-1">
														Права и обязанности администрации
													</button>
												</li>
												<li class="nav-item" role="presentation">
													<button class="nav-link text-center w-100" id="bans-tab" data-bs-toggle="tab" data-bs-target="#bans-tab-pane" type="button" role="tab" aria-controls="bans-tab-pane" aria-selected="false" tabindex="-1">
														Запреты и наказания
													</button>
												</li>
											</ul>
										</div>
										<div class="col-12 col-lg-9 col-xl-10 py-4">
											<div class="tab-content" id="generalRulesContent">
												<div class="tab-pane fade show active" id="general-tab-pane" role="tabpanel" aria-labelledby="general-tab" tabindex="0">
													<p>
														<code>1.1</code> Регистрируясь на сервере, вы соглашаетесь со всеми
														правилами предоставленными в этом списке, правами описанными ниже и
														обязанностями<br>
														<code>1.2</code> Незнание правил не освобождает от ответственности<br>
														<code>1.3</code> При вводе на сайте не верного ника администрация не
														отвечает за последствия покупки доната на этот ник<br>
														<code>1.4</code> Передача/продажа аккаунтов сторонним лицам строго
														запрещена<br>
														<code>1.5</code> Администрация оставляет за собой право в одностороннем
														порядке изменять текущие правила без уведомления пользователей
														посредством группы VK<br>
														<code>1.6</code> Администрация ведет управление игровыми процессами и
														всем проектом - исключительно по своему усмотрению<br>
														<code>1.7</code> Так как не всегда удается определить нарушение правил
														пользователем, окончательное решение остается за Администраторами
														проекта<br>
													</p>
												</div>
												<div class="tab-pane fade" id="rights-tab-pane" role="tabpanel" aria-labelledby="rights-tab" tabindex="0">
													<p>
														<code>2.1</code> Игрок полностью отвечает за надежность своего пароля и
														доступа к аккаунту<br>
														<code>2.2</code> Игрок соглашается с тем, что потраченные им средства не
														будут возвращены<br>
														<code>2.3</code> Игроки, имеющие различные привилегии на сервере, ничем
														не отличаются от обычных игроков, кроме привилегий и полностью
														подчиняются правилам проекта<br>
														<code>2.4</code> В случае отсутствия игрока более 3х календарных месяца,
														все его данные, включая постройки на сервере, личный аккаунт и др. могут
														быть удалены, без оповещения его об этом (Если у вас есть донат у вас
														ничего не пропадет)<br>
													</p>
												</div>
												<div class="tab-pane fade" id="admins-tab-pane" role="tabpanel" aria-labelledby="admins-tab" tabindex="0">
													<p>
														<code>3.1</code> Главная администрация проекта является самым высоким по
														званию лицом, которое может не соблюдать данные правила и действовать на
														свое усмотрение<br>
														<code>3.2</code> Администрация не несет ответственности за аккаунты
														игроков, включая социальную инженерию, вирусы, подбор пароля и т.п<code>.</code><br>
														<code>3.3</code> Все полученные администрацией средства, являются
														добровольным пожертвованием и не подлежат возврату<br>
														<code>3.4</code> Администрация вправе выдавать любое наказание<br>
														<code>3.5</code> Толкование правил сайта осуществляется только главными
														Администраторами. Любые другие попытки истолковать правила в пользу
														любой из сторон признаются некорректными<br>
														<code>3.6</code> Жалобы на администрацию не принимаются<br>
														<code>3.7</code> Администрация вправе забирать привилегии \ отказывать в
														обслуживании игрокам без объяснения причины<br>
														<code>3.8</code> Администрация имеет право не объяснять причины
														блокировки аккаунтов.<br>
														<code>3.9</code> Администратор вправе изъять у пользователя любое
														имущество, если пользователь не сможет доказать его честное (без
														использования запрещенных дополнительных программных средств – читов и
														т.д.) происхождение <br>
													</p>
												</div>
												<div class="tab-pane fade" id="bans-tab-pane" role="tabpanel" aria-labelledby="bans-tab" tabindex="0">
													<p>
                                                       <code>4.1</code> Затрагивание семьи в оскорбительной форме - родных, национальности, языка, религий, а также межрасовая-народная рознь. <i class="text-muted"> (Временный мут до 3 часов)</i><br>
                                                        <code>4.2</code> Гриферство от креатива <i class="text-muted"> (Наказание: Блокировка аккаунта до 5 часов)</i><br>
                                                        <code>4.3</code> Подстрекательство игроков на нарушение правил сервера, в т.ч провокация. <i class="text-muted"> (Наказание: Временный мут до 1 дня)</i><br>
                                                        <code>4.4</code> Неприличные/оскорбительные постройки или постройки, которые портят архитектуру игровой карты, такие как: столбы/лестницы в небо, коробки, застройка чужих построек и т.д. <i class="text-muted"> (Наказание: Снос постройки + бан до 4 часов)</i><br>
                                                        <code>4.5</code> Зазывать на ловушки <i class="text-muted"> (Наказание: Блокировка аккаунта на 30 мин. + удаление ловушки)</i><br>
                                                        <code>4.6</code> Флуд, мат, оскорбление, капс, попрошайничество в чате <i class="text-muted"> (Наказание: Предупреждение, временный мут до 60 мин.)</i><br>
                                                        <code>4.7</code> Продавать/передавать аккаунты <i class="text-muted"> (Наказание: Перманентный бан аккаунта.)</i><br>
                                                        <code>4.8</code> Препятствие нормальной игре / помеха в регионе / багоюз <i class="text-muted"> (Наказание: Блокировка аккаунта на 3 час)</i><br>
                                                        <code>4.9</code> Необоснованное наказание игроков <i class="text-muted"> (Наказание: За мут/варн/кик/jail без причины - Бан до 1 часа, За бан без причины - Бан до 8 часов)</i><br>
                                                        <code>4.10</code> Оскорблять проект и его администрацию <i class="text-muted"> (Наказание: Блокировка аккаунта на 3 дня)</i><br>
                                                        <code>-</code> Оскорбление Модераторов / провокация <i class="text-muted"> (Наказание: Временный мут, бан до 5 часов)</i><br>
                                                        <code>4.11</code> Разбан/размут нарушителя. <i class="text-muted"> (Наказание: Блокировка аккаунта на 8 часов)</i><br>
                                                        <code>4.12</code> Вводить в заблуждение администрацию/модерацию проекта; (Подделка скриншотов). <i class="text-muted"> (Наказание: Блокировка аккаунта до 2 дней)</i><br>
                                                        <code>4.13</code> Подделка сообщений <i class="text-muted"> (Наказание: Блокировка аккаунта от 2 до 5 дней.)</i><br>
                                                        <code>4.14</code> Использование читов в пвп <i class="text-muted"> (Наказание: Блокировка аккаунта на 30 дней)</i><br>
                                                        <code>4.15</code> Использование возможностей доната в корыстных целях (в пвп, полете и т.п; перо разрешено, выдача некорректных ников). <i class="text-muted"> (Наказание: Блокировка аккаунта до 1 дня)</i><br>
                                                        <code>4.16</code> Реклама других проектов в любом виде <i class="text-muted"> (Наказание: Перманентный бан аккаунта / Бан по IP)</i><br>
                                                        <code>4.17</code> Любое вредительство работе сервера т.е. устраивание лагов/вылетов и т.д. <i class="text-muted"> (Наказание: Блокировка аккаунта до 7 дней)</i><br>
                                                        <code>4.18</code> Мошенничество и сделки, связанные с продажей игровых ценностей за реальные деньги. <i class="text-muted"> (Наказание: Перманентный бан аккаунта / Бан по IP)</i><br>
                                                        <code>4.19</code> Порча/изменение/снос спавна, в т.ч.его поджигание. <i class="text-muted"> (Наказание: Перманентный бан аккаунта / снятие доната)</i><br>
                                                        <code>4.20</code> Выдавать себя за персонал или администрацию. <i class="text-muted"> (Наказание: Блокировка аккаунта до 7 дней)</i><br>
													</p>
												</div>
											</div>
										</div>
									</div>
								</div>
								<!-- Гриферские правила -->
								<div class="tab-pane fade" id="grief-rules-tab-pane" role="tabpanel" aria-labelledby="grief-rules-tab" tabindex="0">
									<div class="row">
										<div class="col-12 col-lg-2 py-4">
											<ul class="nav flex-column nav-pills gap-2" id="griefRulesTab" role="tablist">
												<li class="nav-item" role="presentation">
													<button class="nav-link active text-center w-100" id="grief-general-tab" data-bs-toggle="tab" data-bs-target="#grief-general-tab-pane" type="button" role="tab" aria-controls="grief-general-tab-pane" aria-selected="true">
														Основное
													</button>
												</li>
												<li class="nav-item" role="presentation">
													<button class="nav-link text-center w-100" id="grief-rights-tab" data-bs-toggle="tab" data-bs-target="#grief-rights-tab-pane" type="button" role="tab" aria-controls="grief-rights-tab-pane" aria-selected="false" tabindex="-1">
														Права и обязанности игроков
													</button>
												</li>
												<li class="nav-item" role="presentation">
													<button class="nav-link text-center w-100" id="grief-bans-tab" data-bs-toggle="tab" data-bs-target="#grief-bans-tab-pane" type="button" role="tab" aria-controls="grief-bans-tab-pane" aria-selected="false" tabindex="-1">
														Запреты и наказания
													</button>
												</li>
												<li class="nav-item" role="presentation">
													<button class="nav-link text-center w-100" id="grief-moders-tab" data-bs-toggle="tab" data-bs-target="#grief-moders-tab-pane" type="button" role="tab" aria-controls="grief-moders-tab-pane" aria-selected="false" tabindex="-1">
														Правила для модераторов
													</button>
												</li>
											</ul>
										</div>
										<div class="col-10 py-4">
											<div class="tab-content" id="griefRulesTabContent">
												<div class="tab-pane fade show active" id="grief-general-tab-pane" role="tabpanel" aria-labelledby="grief-general-tab" tabindex="0">
													<p>
														<code>1.1</code> Регистрируясь на сервере, вы соглашаетесь со всеми
														правилами предоставленными в этом списке, правами описанными ниже и
														обязанностями<br>
														<code>1.2</code> Незнание правил не освобождает от ответственности<br>
														<code>1.3</code> При вводе на сайте не верного ника администрация не
														отвечает за последствия покупки доната на этот ник<br>
														<code>1.4</code> Передача/продажа аккаунтов сторонним лицам строго
														запрещена<br>
														<code>1.5</code> Администрация оставляет за собой право в одностороннем
														порядке изменять текущие правила без уведомления пользователей
														посредством группы VK<br>
														<code>1.6</code> Администрация ведет управление игровыми процессами и
														всем проектом - исключительно по своему усмотрению<br>
														<code>1.7</code> Так как не всегда удается определить нарушение правил
														пользователем, окончательное решение остается за Администраторами
														проекта<br>
													</p>
												</div>
												<div class="tab-pane fade" id="grief-rights-tab-pane" role="tabpanel" aria-labelledby="grief-rights-tab" tabindex="0">
													<p>
														<code>2.1</code> Игрок полностью отвечает за надежность своего пароля и
														доступа к аккаунту<br>
														<code>2.2</code> Игрок соглашается с тем, что потраченные им средства не
														будут возвращены<br>
														<code>2.3</code> Игроки, имеющие различные привилегии на сервере, ничем
														не отличаются от обычных игроков, кроме привилегий и полностью
														подчиняются правилам проекта<br>
														<code>2.4</code> В случае отсутствия игрока более 3х календарных месяца,
														все его данные, включая постройки на сервере, личный аккаунт и др. могут
														быть удалены, без оповещения его об этом (Если у вас есть донат у вас
														ничего не пропадет)<br>
													</p>
												</div>
												<div class="tab-pane fade" id="grief-bans-tab-pane" role="tabpanel" aria-labelledby="grief-bans-tab" tabindex="0">
													<p>
                                                        <code>3.1</code> Использование / Хранение Чит-клиентов, Чит-Модификаций; <i class="text-muted"> (Наказание: Перманентный бан аккаунта.)</i><br>
                                                        <code>3.2</code> Обход наказания, выданным модератором/администратором; <i class="text-muted"> (Наказание: Если вы создаете новый аккаунт для обхода, он также будет заблокирован.)</i><br>
                                                        <code>3.3</code> Подстрекательство на нарушение правил; <i class="text-muted"> (Наказание: Временный мут до 3 часов.)</i><br>
                                                        <code>3.4</code> Затрагивание семьи в оскорбительной форме - родных, национальности, языка, религий, а также межрасовая-народная рознь; <i class="text-muted"> (Наказание: Временный мут до 3 часов.)</i><br>
                                                        <code>3.5</code> Оскорбление модерации; <i class="text-muted"> (Наказание: Временный мут до 3 часов)</i><br>
                                                        <code>3.6</code> Флуд, спам, оскорбление игроков, попрошайничество в чате/лс; <i class="text-muted"> (Наказание: Временный мут до 2 часов.)</i><br>
                                                        <code>3.7</code> Передача / Продажа аккаунта сторонним лицам; <i class="text-muted"> (Наказание: Перманентный бан аккаунта.)</i><br>
                                                        <code>3.8</code> Необоснованное наказание игроков;<br>
                                                        <i class="text-muted"> (Наказание: За кик без причины/доказательств - блокировка аккаунта до 2 часов,)</i><br>
                                                        <i class="text-muted"> (Наказание: За мут без причины/доказательств - блокировка аккаунта до 4 часов,)</i><br>
                                                        <i class="text-muted"> (Наказание: За бан без причины/доказательств - блокировка аккаунта до 1 дня))</i><br>
                                                        <code>3.9</code> Оскорбление проекта/администрации проекта; <i class="text-muted"> (Наказание: Блокировка аккаунта до 7 дней.)</i><br>
                                                        <code>3.10</code> Вводить в заблуждение, администрацию/модерацию проекта; (Подделка скриншотов) <i class="text-muted"> (Наказание: Блокировка аккаунта до 2 дней.)</i><br>
                                                        <code>3.11</code> Использование уязвимости сервера; (Багов, Дюпов) <i class="text-muted"> (Наказание: Бан до 14 дней)</i><br>
                                                        <code>3.12</code> Выдача себя за администрацию/модерацию проекта; <i class="text-muted"> (Наказание: Блокировка аккаунта до 7 дней)</i><br>
                                                        <code>3.13</code> Ставить ники, которые оскорбляют игроков/модерацию/администрацию проекта; <i class="text-muted"> (Блокировка аккаунта Перманентом)</i><br>
                                                        <code>3.14</code> Реклама других проектов в любом виде; <i class="text-muted"> (Наказание: Блокировка аккаунта Перманентом \ по IP)</i><br>
                                                        <code>3.15</code> Сделки, связанные с продажей игровых ценностей за реальные деньги; <i class="text-muted"> (Наказание: Блокировка аккаунтов Перманентом \ по IP)</i><br>
                                                        <code>3.16</code> Разбан/размут нарушителя.; <i class="text-muted"> (Наказание: Блокировка аккаунта на 8 часов)</i><br>
                                                        <code>3.17</code> Устанавливать объекты для создания лагов на сервере; <i class="text-muted"> (Наказание: Предупреждение, Блокировка аккаунта до 7 дней)</i><br>
                                                        <code>3.18</code> Многочисленное нарушение правил проекта/вредительство; <i class="text-muted"> (Наказание: Блокировка аккаунта от 7 дней до Перманентного \ по IP)</i><br>
                                                        <code>3.19</code> Использовать возможности доната в корыстных целях; (Спам/флуд командами) <i class="text-muted"> (Наказание: Предупреждение / Блокировка аккаунта до 1 дня.)</i><br>
                                                        <code>3.20</code> Тим с читером; <i class="text-muted"> (Наказание: Перманентный бан аккаунта.)</i><br>
													</p>
												</div>
												<div class="tab-pane fade" id="grief-moders-tab-pane" role="tabpanel" aria-labelledby="grief-moders-tab" tabindex="0">
													<p>
                                                        <code>4.1</code> При выдаче бана/мута/кика/предупреждения модератор обязан иметь скриншот/видеозапись нарушения;<br>
                                                        <code>4.2</code> Запрещено использование игровых полномочий во вред серверу;<br>
                                                        <code>4.3</code> Запрещено создавать помехи для игры при телепортации к другому игроку;<br>
                                                        <code>4.4</code> Адекватно вести себя, как в чате, так и в игре;<br>
                                                        <code>4.5</code> Знать свои прямые обязанности и выполнять их;<br>
                                                        <code>4.6</code> Соблюдать устав правил;<br>
                                                        <code>4.7</code> Запрещено преждевременное снятие наказания;<br>
                                                        <code>4.8</code> Запрещено оскорблять Игроков сервера; (распространяется на соц.сети)<br>
													</p>
												</div>
											</div>
										</div>
									</div>
								</div>
								<!-- Правила bedwars -->
							</div>
						</div>
					</div>
					<!-- <div class="modal-footer">
						<button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Закрыть</button>
					</div> -->
				</div>
			</div>
		</div>
		<!-- Возможности доната -->
		<div class="modal fade" id="modalRanks" tabindex="-1" aria-labelledby="modalLabel" aria-hidden="true">
			<div class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-lg">
				<div class="modal-content border-0" style="height: 70%;">
					<div class="modal-header">
						<h1 class="modal-title fs-5" id="modalLabel">Возможности доната</h1>
						<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
					</div>
					<div class="modal-body">
						<div class="container-fluid">
							<ul class="nav nav-tabs" id="ranksTabs" role="tablist">
								<li class="nav-item" role="presentation">
									<button class="nav-link active" id="survival-ranks-tab" data-bs-toggle="tab" data-bs-target="#survival-ranks-tab-pane" type="button" role="tab" aria-controls="survival-ranks-tab-pane" aria-selected="true">
										Выживание
									</button>
								</li>
								<li class="nav-item" role="presentation">
									<button class="nav-link" id="grief-ranks-tab" data-bs-toggle="tab" data-bs-target="#grief-ranks-tab-pane" type="button" role="tab" aria-controls="grief-ranks-tab-pane" aria-selected="false" tabindex="-1">
										Гриферский
									</button>
								</li>
								<li class="nav-item" role="presentation">
									<button class="nav-link" id="bedwars-ranks-tab" data-bs-toggle="tab" data-bs-target="#bedwars-ranks-tab-pane" type="button" role="tab" aria-controls="bedwars-ranks-tab-pane" aria-selected="false" tabindex="-1">
										BedWars
									</button>
								</li>
							</ul>
							<div class="tab-content" id="ranksTabsContent">
								<!-- Выживание -->
								<div class="tab-pane fade show active" id="survival-ranks-tab-pane" role="tabpanel" aria-labelledby="survival-ranks-tab" tabindex="0">
									<div class="row">
										<div class="col-12 col-lg-3 py-4" style="max-height: 50vh; overflow-y: auto; overflow-x: hidden">
											<ul class="nav nav-pills d-grid d-lg-flex" id="survivalRanksTab" role="tablist" style="grid-template-areas: &#39;a a a&#39;; gap: 0.25rem">
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link active text-center w-100" id="survival-vip-tab" data-bs-toggle="tab" data-bs-target="#survival-vip-tab-pane" type="button" role="tab" aria-controls="survival-vip-tab-pane" aria-selected="true">
														Вип
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-premium-tab" data-bs-toggle="tab" data-bs-target="#survival-premium-tab-pane" type="button" role="tab" aria-controls="survival-premium-tab-pane" aria-selected="false" tabindex="-1">
														Премиум
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-creative-tab" data-bs-toggle="tab" data-bs-target="#survival-creative-tab-pane" type="button" role="tab" aria-controls="survival-creative-tab-pane" aria-selected="false" tabindex="-1">
														Креатив
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-legenda-tab" data-bs-toggle="tab" data-bs-target="#survival-legenda-tab-pane" type="button" role="tab" aria-controls="survival-legenda-tab-pane" aria-selected="false" tabindex="-1">
														Легенда
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-moder-tab" data-bs-toggle="tab" data-bs-target="#survival-moder-tab-pane" type="button" role="tab" aria-controls="survival-moder-tab-pane" aria-selected="false" tabindex="-1">
														Модер
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-admin-tab" data-bs-toggle="tab" data-bs-target="#survival-admin-tab-pane" type="button" role="tab" aria-controls="survival-admin-tab-pane" aria-selected="false" tabindex="-1">
														Админ
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-gladmin-tab" data-bs-toggle="tab" data-bs-target="#survival-gladmin-tab-pane" type="button" role="tab" aria-controls="survival-gladmin-tab-pane" aria-selected="false" tabindex="-1">
														Гл. Админ
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-enigma-tab" data-bs-toggle="tab" data-bs-target="#survival-enigma-tab-pane" type="button" role="tab" aria-controls="survival-enigma-tab-pane" aria-selected="false" tabindex="-1">
														Энигма
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-imperator-tab" data-bs-toggle="tab" data-bs-target="#survival-imperator-tab-pane" type="button" role="tab" aria-controls="survival-imperator-tab-pane" aria-selected="false" tabindex="-1">
														Император
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-deluxe-tab" data-bs-toggle="tab" data-bs-target="#survival-deluxe-tab-pane" type="button" role="tab" aria-controls="survival-deluxe-tab-pane" aria-selected="false" tabindex="-1">
														Делюкс
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-pomoshnik-tab" data-bs-toggle="tab" data-bs-target="#survival-pomoshnik-tab-pane" type="button" role="tab" aria-controls="survival-pomoshnik-tab-pane" aria-selected="false" tabindex="-1">
														Помощник
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-opka-tab" data-bs-toggle="tab" data-bs-target="#survival-opka-tab-pane" type="button" role="tab" aria-controls="survival-opka-tab-pane" aria-selected="false" tabindex="-1">
														Опка
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-helper-tab" data-bs-toggle="tab" data-bs-target="#survival-helper-tab-pane" type="button" role="tab" aria-controls="survival-helper-tab-pane" aria-selected="false" tabindex="-1">
														Хелпер
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-blaze-tab" data-bs-toggle="tab" data-bs-target="#survival-blaze-tab-pane" type="button" role="tab" aria-controls="survival-blaze-tab-pane" aria-selected="false" tabindex="-1">
														Блейз
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-antigrief-tab" data-bs-toggle="tab" data-bs-target="#survival-antigrief-tab-pane" type="button" role="tab" aria-controls="survival-antigrief-tab-pane" aria-selected="false" tabindex="-1">
														АнтиГрифер
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-vlastelin-tab" data-bs-toggle="tab" data-bs-target="#survival-vlastelin-tab-pane" type="button" role="tab" aria-controls="survival-vlastelin-tab-pane" aria-selected="false" tabindex="-1">
														Властелин
													</button>
												</li>

												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="survival-owner-tab" data-bs-toggle="tab" data-bs-target="#survival-owner-tab-pane" type="button" role="tab" aria-controls="survival-owner-tab-pane" aria-selected="false" tabindex="-1">
														Владелец
													</button>
												</li>
											</ul>
										</div>
										<div class="col-9 py-4">
											<div class="tab-content" id="survivalRanksTabContent">
												<div class="tab-pane fade show active" id="survival-vip-tab-pane" role="tabpanel" aria-labelledby="survival-vip-tab" tabindex="0">
													<ul>
														<li>Возможность получить набор /kit vip</li>
														<li>Возможность получить машину /auto</li>
														<li>Возможность отключения тел-ции /tptoggle</li>
														<li>Возможность проверить пинг /ping</li>
														<li>Возможность очистить инвентарь /ci</li>
														<li>Возможность эндер сундук /echest</li>
														<li>Возможность одеть блок на голову /hat</li>
														<li>Возможность вернуться назад /back</li>
														<li>Возможность игнорировать игрока /ignore</li>
														<li>Возможность заходить на полный сервер</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-premium-tab-pane" role="tabpanel" aria-labelledby="survival-premium-tab" tabindex="0">
													<ul>
														<li>Возможность получить набор /kit prem</li>
														<li>Возможность получить ховербайк /auto</li>
														<li>Возможность получить байк /auto</li>
														<li>Возможность включить полёт /fly</li>
														<li>Возможность починить вещи /fix all</li>
														<li>Возможность включить бессмертие /god</li>
														<li>Возможность открыть верстак /wbench</li>
														<li>Возможность посмотреть крафт /recipe</li>
														<li>Возможность восстановить голод /feed</li>
														<li>Возможность встать в афк режим /afk</li>
														<li>Возможность установить 4 дома /sethome</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-creative-tab-pane" role="tabpanel" aria-labelledby="survival-creative-tab" tabindex="0">
													<ul>
														<li>Возможность выдать джетпак /feather</li>
														<li>Возможность стрельнуть /kittycannon</li>
														<li>Возможность узнать айди /durability</li>
														<li>Возможность включить креатив /gm 1</li>
														<li>Возможность включить приключ. /gm 2</li>
														<li>Возможность выключить креатив /gm 0</li>
														<li>Возможность много точек дома /sethome</li>
														<li>Возможность посмотреть игроков /near</li>
														<li>Возможность персональное время /ptime</li>
														<li>Возможность выдать опыт exp</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-legenda-tab-pane" role="tabpanel" aria-labelledby="survival-legenda-tab" tabindex="0">
													<ul>
														<li>Возможность использовать админ чат /ac</li>
														<li>Возможность включить невидимку /vanish</li>
														<li>Возможность телепорт к другим /tp</li>
														<li>Возможность телепорт к себе /tphere</li>
														<li>Возможность дюпнуть предмет /more</li>
														<li>Возможность инфо о сервере /gc</li>
														<li>Возможность сменить погоду /weather</li>
														<li>Возможность изменить время мира /time</li>
														<li>Возможность телепортировать блок /jump</li>
														<li>Возможность игнорировать игрока /ignore</li>
														<li>Возможность несколько точек дома /sethome</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-moder-tab-pane" role="tabpanel" aria-labelledby="survival-moder-tab" tabindex="0">
													<ul>
														<li>Возможность телепорт наверх /etop</li>
														<li>Возможность телепорт координат /tppos</li>
														<li>Возможность выдать опыт игроку /exp</li>
														<li>Возможность вылечить игрока /heal</li>
														<li>Возможность проверить баланс /balance</li>
														<li>Возможность показать топ богачей /baltop</li>
														<li>Возможность создатель варп /setwarp</li>
														<li>Возможность удалить свой варп /delwarp</li>
														<li>Возможность посмотреть свои варпы /mywarps</li>
														<li>Возможность запустить огненный шар /fireball</li>
														<li>Возможность несколько точек дома /sethome</li>
														<li>Возможность видеть игроков в ванише</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-admin-tab-pane" role="tabpanel" aria-labelledby="survival-admin-tab" tabindex="0">
													<ul>
														<li>Возможность поджечь игрока /burn</li>
														<li>Возможность узнать координаты /getpos</li>
														<li>Возможность поставить солнце /sun</li>
														<li>Возможность поставить дождь /rain</li>
														<li>Возможность включить день /day</li>
														<li>Возможность включить ночь /night</li>
														<li>Изменить название предмета /setname</li>
														<li>Изменить описание предмета /setlore</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-gladmin-tab-pane" role="tabpanel" aria-labelledby="survival-gladmin-tab" tabindex="0">
													<ul>
														<li>Возможность редактировать книгу /book</li>
														<li>Возможность добавить эффект /potion</li>
														<li>Возможность смена погоды /pweather</li>
														<li>Возможность узнать координаты /getpos   </li>
														<li>Возможность изменить погоду /weather</li>
														<li>Возможность ударить молнией /lightning</li>
														<li>Возможность сделать мини-объяление /me</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-enigma-tab-pane" role="tabpanel" aria-labelledby="survival-enigma-tab" tabindex="0">
													<ul>
														<li>Возможность выдать предупреждение /warn</li>
														<li>Возможность убрать предупреждение /unwarn</li>
														<li>Возможность отправить запрос тп /tpahere</li>
														<li>Возможность последних заходов /seen</li>
														<li>Возможность узнать реальное имя /realname</li>
														<li>Возможность разбанить игрока /unban</li>
														<li>Возможность поджечь игрока /burn</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-imperator-tab-pane" role="tabpanel" aria-labelledby="survival-imperator-tab" tabindex="0">
													<ul>
														<li>Доступ к просмотру чужих сундуков в рг</li>
														<li>Возможность использовать сет //set</li>
														<li>Возможность забанить игрока /ban</li>
														<li>Возможность телепорт к себе /tphere</li>
														<li>Возможность бесконечных блоков /unlimited</li>
														<li>Возможность дать мут игроку /mute</li>
														<li>Возможность кикнуть игрока /kick</li>
														<li>Возможность снять мут /unmute</li>
														<li>Возможность снять бан /unban</li>
														<li>Возможность дать fly игроку /fly</li>
														<li>Возможность зачаровать /enchant</li>
														<li>Возможность поджечь игрока /burn</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-deluxe-tab-pane" role="tabpanel" aria-labelledby="survival-deluxe-tab" tabindex="0">
													<ul>
														<li>Доступ к просмотру чужих сундуков в рг</li>
														<li>Возможность сетать //set <i class="text-mute">(увеличен х2)</i></li>
														<li>Вечный иммунитет от бана/кика/мута и т.д.</li>
														<li>Возможность превратить в блоки /compact</li>
														<li>Возможность писать объявление /bc</li>
														<li>Возможность забанить игрока /ban</li>
														<li>Возможность дать мут игроку /mute</li>
														<li>Возможность кикнуть игрока /kick</li>
														<li>Возможность снять мут /unmute</li>
														<li>Возможность снять бан /unban</li>
														<li>Возможность изменить ник /nick</li>
														<li>Возможность сделать динамит /tnt</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-pomoshnik-tab-pane" role="tabpanel" aria-labelledby="survival-pomoshnik-tab" tabindex="0">
													<ul>
														<li>Доступ к просмотру чужих сундуков в рг</li>
														<li>Полный доступ к флагам /rg flag</li>
														<li>Возможность дать денег /eco give</li>
														<li>Возможность сетать //set <i class="text-mute">(увеличен х3)</i></li>
														<li>Возможность телепорт к себе /tphere</li>
														<li>Возможность включить нано-броню /guard</li>
														<li>Возможность выдать себе предмет /i</li>
														<li>Возможность выдать игроку предмет /give</li>
														<li>Возможность включить радужную броню /ra</li>
														<li>Возможность включить диско броню /da</li>
														<li>Возможность узнать азимут /compass</li>
														<li>Возможность узнать высоту моря /depth</li>
														<li>Возможность узнать инфо региона /rg info</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-opka-tab-pane" role="tabpanel" aria-labelledby="survival-opka-tab" tabindex="0">
													<ul>
														<li>Стикеры в табе /sticktab</li>
														<li>Стикеры в чате /stickchat</li>
														<li>Слова в чате /chatword</li>
														<li>Слова в табе /tabword</li>
														<li>75% команд сервера</li>
														<li>Доступ к просмотру чужих сундуков в рг</li>
														<li> У вас иммунитет от бана <i class="text-mute">(невозможно забанить)</i></li>
														<li>Возможность сетать //set<i class="text-mute">(увеличен х5)</i></li>
														<li>Возможность телепорт игрока на спавн /spawn</li>
														<li>Возможность следить за сообщениями /socialspy</li>
														<li>Возможность телепорт к игроку с tptoggle /tpo</li>
														<li>Возможность дать fly другу /fly</li>
														<li>Доступ к цветному чату &amp; + Цифра цвета</li>
														<li>Возможно использовать цвета на табличках</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-helper-tab-pane" role="tabpanel" aria-labelledby="survival-helper-tab" tabindex="0">
													<ul>
														<li>85% команд сервера</li>
														<li>Выдаются почти все команды сервера</li>
														<li>Возможность мини-консоли /console</li>
														<li>Возможность дать фейк-оп /fakeop</li>
														<li>Возможность сделать стены //walls</li>
														<li>Возможность сетать //set<i class="text-mute">(увеличен х10)</i></li>
														<li>Возможность убрать воду //drain</li>
														<li>Возможность забанить по IP /ipban</li>
														<li>Возможность забанить навсегда /ban</li>
														<li>Возможность замутить навсегда /mute</li>
														<li>Возможность делать пирамиду //pyramid</li>
														<li>Возможность делать любой ник /nick</li>
														<li>Возможность скопировать постройку //copy</li>
														<li>Возможность встьавить постройку //paste</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-blaze-tab-pane" role="tabpanel" aria-labelledby="survival-blaze-tab" tabindex="0">
													<ul>
														<li>99% команд сервера</li>
														<li>Вам доступны все команды сервера</li>
														<li>В два раза понижены задержки на все команды</li>
														<li>Вы получаете звездочку в pex</li>
														<li>Вы получаете полную опку<i class="text-mute">(без лимита)</i></li>
														<li>Полный доступ к приватам<i class="text-mute">(без лимита)</i></li>
														<li>Создать собственную голограмму /holo</li>
														<li>Включить свечение /glow</li>
														<li>Смайлики для чата /emoji</li>
														<li>Установить цвет текста в чате /chatcolor</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-antigrief-tab-pane" role="tabpanel" aria-labelledby="survival-antigrief-tab" tabindex="0">
													<ul>
														<li>Полный доступ WorldEdit <i class="text-mute">(топорик)</i></li>
														<li>Доступ к приватам <i class="text-mute">(3 в день)</i></li>
														<li>Возможность выдать бан /ban <i class="text-mute">(на 24 часа)</i> </li>
														<li>Возможность выдать мут /mute <i class="text-mute">(на 24 часа)</i> </li>
														<li>Возможность ставить любой ник /nick</li>
														<li>Возможность выдавать донат /grant</li>
														<li>Возможность посадить в тюрьму /jail</li>
														<li>Возможность изменить скорость /speed</li>
														<li>Возможность заспавнить моба /spawnmob</li>
														<li>Возможность сменить цвет префикса /color</li>
														<li>Вы будете в начале списка игроков <i class="text-mute">(таб)</i> </li>
														<li>Приоритетная поддержка, если вы забудете</li>
														<li>пароль - мы восстановим вам аккаунт <i class="text-mute">(по чеку)</i> </li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-vlastelin-tab-pane" role="tabpanel" aria-labelledby="survival-vlastelin-tab" tabindex="0">
													<ul>
														<li>Расширенный доступ к приватам <i class="text-mute">(9 в день)</i></li>
														<li>Сохранить свою постройку навсегда /rgsaver</li>
														<li>Превратиться в любой блок /dblock</li>
														<li>Установить сообщение при входе /jm</li>
														<li>Установить любой цвет свечения /glowcolor</li>
														<li>Установить уникальный суффикс /vsuffix</li>
														<li>Сменить цвет префикса /vcolor</li>
														<li>Возможность превратиться в моба /dis</li>
														<li>Возможность забанить людей с иммунитетом</li>
														<li>Возможность выдать бан /ban (на 3 дня)</li>
														<li>Возможность выдать мут /mute (на 3 дня)</li>
														<li>Возможность выдавать донат /grant</li>
														<li>Приоритетная поддержка, если вы забудете</li>
														<li>пароль - мы восстановим вам аккаунт <i class="text-mute">(по чеку)</i></li>
													</ul>
												</div>
												<div class="tab-pane fade" id="survival-owner-tab-pane" role="tabpanel" aria-labelledby="survival-owner-tab" tabindex="0">
													<ul>
														<li>Вам РЕАЛЬНО выдаются все команды сервера</li>
														<li>Можно сменить префикс в табе /tab prefix</li>
														<li>Можно сменить префикс в чате /chat prefix</li>
														<li>Вы сможете писать заблокированные слова в чат</li>
														<li>Полный доступ к топорику <i class="text-mute">(WorldEdit)</i></li>
														<li> У вас будет связь с создателем <i class="text-mute">(добавит в друзья)</i></li>
														<li>Безлимитный доступ ко всем регионам</li>
														<li> Вам доступны все команды сервера <i class="text-mute">(Даже опасные)</i></li>
														<li>Вы сможете выдать донат другу /grant</li>
														<li>Вы будете в команде Администрации сервера.</li>
														<li>Можно сходить с создателем в Discord</li>
														<li>С Вас сняты все задержки на команды</li>
														<li>Вы получаете звездочку в pex</li>
														<li>Вы получаете полную опку <i class="text-mute">(без лимита)</i></li>
													</ul>
												</div>
											</div>
										</div>
									</div>
								</div>
								<!-- Гриферский -->
								<div class="tab-pane fade" id="grief-ranks-tab-pane" role="tabpanel" aria-labelledby="grief-ranks-tab" tabindex="0">
									<div class="row">
										<div class="col-12 col-lg-3 py-4" style="max-height: 50vh; overflow-y: auto; overflow-x: hidden">
											<ul class="nav nav-pills d-grid d-lg-flex" id="griefRanksTab" role="tablist" style="grid-template-areas: &#39;a a a&#39;; gap: 0.25rem">
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link active text-center w-100" id="grief-silver-tab" data-bs-toggle="tab" data-bs-target="#grief-silver-tab-pane" type="button" role="tab" aria-controls="grief-silver-tab-pane" aria-selected="true">
														Silver
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-supreme-tab" data-bs-toggle="tab" data-bs-target="#grief-supreme-tab-pane" type="button" role="tab" aria-controls="grief-supreme-tab-pane" aria-selected="false" tabindex="-1">
														Supreme
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-wither-tab" data-bs-toggle="tab" data-bs-target="#grief-wither-tab-pane" type="button" role="tab" aria-controls="grief-wither-tab-pane" aria-selected="false" tabindex="-1">
														Wither
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-hero-tab" data-bs-toggle="tab" data-bs-target="#grief-hero-tab-pane" type="button" role="tab" aria-controls="grief-hero-tab-pane" aria-selected="false" tabindex="-1">
														Hero
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-avenger-tab" data-bs-toggle="tab" data-bs-target="#grief-avenger-tab-pane" type="button" role="tab" aria-controls="grief-avenger-tab-pane" aria-selected="false" tabindex="-1">
														Avenger
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-legend-tab" data-bs-toggle="tab" data-bs-target="#grief-legend-tab-pane" type="button" role="tab" aria-controls="grief-legend-tab-pane" aria-selected="false" tabindex="-1">
														Legend
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-phantom-tab" data-bs-toggle="tab" data-bs-target="#grief-phantom-tab-pane" type="button" role="tab" aria-controls="grief-phantom-tab-pane" aria-selected="false" tabindex="-1">
														Phantom
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-phoenix-tab" data-bs-toggle="tab" data-bs-target="#grief-phoenix-tab-pane" type="button" role="tab" aria-controls="grief-phoenix-tab-pane" aria-selected="false" tabindex="-1">
														Phoenix
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="grief-ender-tab" data-bs-toggle="tab" data-bs-target="#grief-ender-tab-pane" type="button" role="tab" aria-controls="grief-ender-tab-pane" aria-selected="false" tabindex="-1">
														Ender
													</button>
												</li>
											</ul>
										</div>
										<div class="col-9 py-4">
											<div class="tab-content" id="griefRanksTabContent">
												<div class="tab-pane fade show active" id="grief-silver-tab-pane" role="tabpanel" aria-labelledby="grief-silver-tab" tabindex="0">
													<ul>
														<li>Доступен набор SILVER /kit silver</li>
														<li>Возможность сменить личное время /ptime</li>
														<li>Возможность открыть верстак /wordkbench</li>
														<li>Возможность открыть эндер-сундук /ec</li>
														<li>Возможность очистить инвентарь /ci</li>
														<li>Возможность отправить запрос тп /tpahere</li>
														<li>Возможность отключить личку /msgtoggle</li>
														<li>Слотов на аукционе: 4</li>
														<li>Регионов для привата: 2 (/rg claim)</li>
														<li>Можно установить 2 сетхома (/sethome)</li>
														<li>Зарплата 50$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-supreme-tab-pane" role="tabpanel" aria-labelledby="grief-supreme-tab" tabindex="0">
													<ul>
														<li>Доступен набор SUPREME /kit supreme</li>
														<li>Возможность одеть блок на голову /hat</li>
														<li>Возможность игнорировать игрока /ignore</li>
														<li>Возможность последних заходов /seen</li>
														<li>Можно сменить погоду себе /pweather</li>
														<li>Стрельнуть котиком /kittycannon</li>
														<li>Стрельнуть пчелкой /beezoka</li>
														<li>Слотов на аукционе: 6</li>
														<li>Регионов для привата: 4 (/rg claim)</li>
														<li>Можно установить 4 сетхома (/sethome)</li>
														<li>Зарплата 100$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-wither-tab-pane" role="tabpanel" aria-labelledby="grief-wither-tab" tabindex="0">
													<ul>
														<li>Доступен набор WITHER /kit wither</li>
														<li>Телепортация поблизости игрока /rtp near</li>
														<li>Возможность написать в админ-чат /ac</li>
														<li>Возможность узнать игроков рядом /near</li>
														<li>Возможность восстановить голод /feed</li>
														<li>Возможность включить свечение /glow</li>
														<li>Возможность потушить себя /ext</li>
														<li>Возможность инфо о сервере /gc</li>
														<li>Слотов на аукционе: 8</li>
														<li>Регионов для привата: 6 (/rg claim)</li>
														<li>Можно установить 6 сетхома (/sethome)</li>
														<li>Зарплата 150$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-hero-tab-pane" role="tabpanel" aria-labelledby="grief-hero-tab" tabindex="0">
													<ul>
														<li>Доступен набор HERO /kit hero</li>
														<li>Возможность писать объявление /mbc</li>
														<li>Можно поменять название предмета /setname</li>
														<li>Можно замаскироваться под игрока /player</li>
														<li>Можно открыть чужой инвентарь /invsee</li>
														<li>Можно отключить телепортацию /tptoggle</li>
														<li>Включить ночное зрение /nightvision</li>
														<li>Можно редактировать таблички командой /sign</li>
														<li>Спавнер выпадет при ломание с шёлк. касанием</li>
														<li>Слотов на аукционе: 12</li>
														<li>Регионов для привата: 8 (/rg claim)</li>
														<li>Можно установить 8 сетхома (/sethome)</li>
														<li>Зарплата 200$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-avenger-tab-pane" role="tabpanel" aria-labelledby="grief-avenger-tab" tabindex="0">
													<ul>
														<li>Доступен набор AVENGER /kit avenger</li>
														<li>Возможность полета на спавне /fly</li>
														<li>Возможность сменить ник /nick</li>
														<li>Возможность поставить солнце /sun</li>
														<li>Возможность поставить дождь /rain</li>
														<li>Возможность включить день /day</li>
														<li>Возможность включить ночь /night</li>
														<li>Посмотреть чужую броню /invsee [ник] -a</li>
														<li>Слотов на аукционе: 22</li>
														<li>Регионов для привата: 50 (/rg claim)</li>
														<li>Можно установить 50 сетхома (/sethome)</li>
														<li>Зарплата 250$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-legend-tab-pane" role="tabpanel" aria-labelledby="grief-legend-tab" tabindex="0">
													<ul>
														<li>Доступен набор LEGEND /kit legend</li>
														<li>Возможность выдать донат /grant</li>
														<li>Возможность кикнуть игрока /kick</li>
														<li>Возможность дать мут игроку /mute</li>
														<li>Возможность снять мут /unmute</li>
														<li>Возможность починить предмет /fix</li>
														<li>Можно читать чужую личку /socialspy</li>
														<li>Можно писать RGB градиентом в чат /chatcolor</li>
														<li>Доступ к цветному чату § + Цифра цвета</li>
														<li>Слотов на аукционе: 30</li>
														<li>Регионов для привата: 99 (/rg claim)</li>
														<li>Можно установить 99 сетхома (/sethome)</li>
														<li>Зарплата 250$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-phantom-tab-pane" role="tabpanel" aria-labelledby="grief-phantom-tab" tabindex="0">
													<ul>
														<li>Доступен набор PHANTOM /kit phantom</li>
														<li>Вечный иммунитет от бана/кика/мута и т.д.</li>
														<li>Возможность выдать донат /grant (увелич. х2)</li>
														<li>Возможность забанить игрока /ban</li>
														<li>Возможность вылечить себя /heal</li>
														<li>Возможность узнать реальное имя /realname</li>
														<li>Возможность накормить игрока /feed &lt;ник&gt;</li>
														<li>Можно починить зачарованный предмет /fix</li>
														<li>Доступны эмодзи для чата /emoji</li>
														<li>Слотов на аукционе: 60</li>
														<li>Регионов для привата: 199 (/rg claim)</li>
														<li>Можно установить 199 сетхома (/sethome)</li>
														<li>Зарплата 300$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-phoenix-tab-pane" role="tabpanel" aria-labelledby="grief-phoenix-tab" tabindex="0">
													<ul>
														<li>Доступен набор PHOENIX /kit phoenix</li>
														<li>Возможность выдать донат /grant (увелич. х3)</li>
														<li>Возможность забанить игрока /ban (увелич. х2)</li>
														<li>Возможность создатель варп /setwarp</li>
														<li>Возможность удалить свой варп /delwarp</li>
														<li>Возможность починить все предметы /fix all</li>
														<li>Возможность получить голову игрока /skull</li>
														<li>Возможность узнать реальное имя /realname</li>
														<li>Слотов на аукционе: 100</li>
														<li>Регионов для привата: 299 (/rg claim)</li>
														<li>Можно установить 299 сетхома (/sethome)</li>
														<li>Зарплата 400$ раз в 5 минут</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="grief-ender-tab-pane" role="tabpanel" aria-labelledby="grief-ender-tab" tabindex="0">
													<ul>
														<li>Доступен набор ENDER /kit ender</li>
														<li>Можно выдать донат /grant (увелич. х5)</li>
														<li>Можно забанить игрока /ban (увелич. х3)</li>
														<li>Можно включить бессмертие /god</li>
														<li>Cменить префикс в табе /tab prefix</li>
														<li>Cменить префикс в чате /chat prefix</li>
														<li>Можно зайти на полный сервер</li>
														<li>Нет кика за АФК</li>
														<li>Слотов на аукционе: 200</li>
														<li>Регионов для привата: 999 (/rg claim)</li>
														<li>Можно установить 999 сетхома (/sethome)</li>
														<li>Зарплата 600$ раз в 5 минут</li>
													</ul>
												</div>
											</div>
										</div>
									</div>
								</div>
								<!-- Bedwars -->
								<div class="tab-pane fade" id="bedwars-ranks-tab-pane" role="tabpanel" aria-labelledby="bedwars-ranks-tab" tabindex="0">
									<div class="row">
										<div class="col-12 col-lg-3 py-4" style="max-height: 50vh; overflow-y: auto; overflow-x: hidden">
											<ul class="nav nav-pills d-grid d-lg-flex" id="bedwarsRanksTab" role="tablist" style="grid-template-areas: &#39;a a a&#39;; gap: 0.25rem">
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link active text-center w-100" id="bedwars-gold-tab" data-bs-toggle="tab" data-bs-target="#bedwars-gold-tab-pane" type="button" role="tab" aria-controls="bedwars-gold-tab-pane" aria-selected="true">
														Gold
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="bedwars-diamond-tab" data-bs-toggle="tab" data-bs-target="#bedwars-diamond-tab-pane" type="button" role="tab" aria-controls="bedwars-diamond-tab-pane" aria-selected="false" tabindex="-1">
														Diamond
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="bedwars-emerald-tab" data-bs-toggle="tab" data-bs-target="#bedwars-emerald-tab-pane" type="button" role="tab" aria-controls="bedwars-emerald-tab-pane" aria-selected="false" tabindex="-1">
														Emerald
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="bedwars-magma-tab" data-bs-toggle="tab" data-bs-target="#bedwars-magma-tab-pane" type="button" role="tab" aria-controls="bedwars-magma-tab-pane" aria-selected="false" tabindex="-1">
														Magma
													</button>
												</li>
												<li class="nav-item w-100" role="presentation">
													<button class="nav-link text-center w-100" id="bedwars-legend-tab" data-bs-toggle="tab" data-bs-target="#bedwars-legend-tab-pane" type="button" role="tab" aria-controls="bedwars-legend-tab-pane" aria-selected="false" tabindex="-1">
														Legend
													</button>
												</li>
											</ul>
										</div>
										<div class="col-9 py-4">
											<div class="tab-content" id="bedwarsRanksTabContent">
												<div class="tab-pane fade show active" id="bedwars-gold-tab-pane" role="tabpanel" aria-labelledby="bedwars-gold-tab" tabindex="0">
													<ul>
														<li>Сидеть в лобби /sit</li>
														<li>Лежать в лобби /lay</li>
														<li>Плевать в лобби /spit</li>
														<li>Пожать руку в лобби /shakehand</li>
														<li>Ползать в лобби /crawl</li>
														<li>Лежать на животе в лобби /bellyflop</li>
														<li>Крутиться в лобби /spin</li>
														<li>Запустить фейерверк в лобби /fw</li>
														<li>Одеть блок на голову в лобби /hat</li>
														<li>Писать в игре и лобби желтым цветом &amp;e</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="bedwars-diamond-tab-pane" role="tabpanel" aria-labelledby="bedwars-diamond-tab" tabindex="0">
													<ul>
														<li>Летать в лобби /fly</li>
														<li>Обнять игрока в лобби /hug</li>
														<li>Укусить игрока в лобби /bite</li>
														<li>Изменить себе время в лобби /ptime</li>
														<li>Изменить себе погоду в лобби /pweather</li>
														<li>Писать в игре и лобби голубым цветом &amp;b</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="bedwars-emerald-tab-pane" role="tabpanel" aria-labelledby="bedwars-emerald-tab" tabindex="0">
													<ul>
														<li>Доступно 5 мобов для превращения /dis</li>
														<li>Изменить скорость в лобби /speed</li>
														<li>Одеть голову другого игрока /skull</li>
														<li>Стрельнуть фаерболом в лобби /fireball</li>
														<li>Писать в игре и лобби зеленым цветом &amp;a</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="bedwars-magma-tab-pane" role="tabpanel" aria-labelledby="bedwars-magma-tab" tabindex="0">
													<ul>
														<li>Доступно 12 мобов для превращения /dis</li>
														<li>Изменить ник в лобби и игре /nick</li>
														<li>Включить свечение в лобби /glow</li>
														<li>Использовать быстрый старт игры</li>
														<li>Писать в игре и лобби оранжевым цветом &amp;6</li>
													</ul>
												</div>
												<div class="tab-pane fade" id="bedwars-legend-tab-pane" role="tabpanel" aria-labelledby="bedwars-legend-tab" tabindex="0">
													<ul>
														<li>Доступны ВСЕ мобы для превращения /dis</li>
														<li>Установить сообщение при входе /jm</li>
														<li>Выбрать цвет префикса в игре и лобби /color</li>
														<li>Выбрать цвет свечения в лобби /glowcolor</li>
														<li>Установить любой ник в игре и лобби /nick</li>
                                                        <li>Отключить рекламу в игре и лобби /settings</li>
														<li>Писать в игре и лобби любым цветом &amp;+цвет</li>
														<li>Понижена задержка на чат (1 сек.)</li>
														<li>Бесконечный выбор карт</li>
														<li>Нет кика за афк</li>
													</ul>
												</div>
											</div>
										</div>
									</div>
								</div>
							</div>
						</div>
					</div>
					<!-- <div class="modal-footer">
						<button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Закрыть</button>
					</div> -->
				</div>
			</div>
		</div>
		<!-- Оплата -->
		<div class="modal fade" id="paymentGateway" tabindex="-1" aria-labelledby="modalLabel" aria-hidden="true">
			<div class="modal-dialog modal-dialog-centered modal-dialog-scrollable" style="--bs-modal-width: 400px">
				<div class="modal-content border-0">
					<div class="modal-header">
						<h1 class="modal-title fs-5 text-center w-100" id="modalLabel">Выберите способ оплаты</h1>
						<button type="button" style="position: absolute; top: 1.5rem; right: 1rem" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
					</div>
					<div class="modal-body">
						<div class="container">
							<div class="row gap-2 justify-content-center" id="paymentButtons">
								<button title="QIWI" data-method="qiwi" class="col-4 rounded-3 btn btn-light p-2 ratio ratio-1x1" style="height: 30%; width: 30%">
									<div class="d-flex flex-column justify-content-center p-2" data-method="qiwi">
										<img src="./MineBlaze - Покупка доната, привилегий, ключей_files/qiwi.svg" data-method="qiwi" alt="">
									</div>
								</button>
								<button title="Банковские карты" data-method="card" class="col-4 rounded-3 btn btn-light p-2 ratio ratio-1x1" style="height: 30%; width: 30%">
									<div class="d-flex flex-column justify-content-center p-2" data-method="card">
										<img src="./MineBlaze - Покупка доната, привилегий, ключей_files/card2.svg" data-method="card" alt="">
									</div>
								</button>
								<button title="ЮMoney" data-method="yandex" class="col-4 rounded-3 btn btn-light p-2 ratio ratio-1x1" style="height: 30%; width: 30%">
									<div class="d-flex flex-column justify-content-center p-2" data-method="yandex">
										<img src="./MineBlaze - Покупка доната, привилегий, ключей_files/yandexmoney.svg" style="max-height: 20%" data-method="yandex" alt="">
									</div>
								</button>
								<button title="Мегафон" data-method="megafon" class="col-4 rounded-3 btn btn-light p-2 ratio ratio-1x1" style="height: 30%; width: 30%">
									<div class="d-flex flex-column justify-content-center p-2" data-method="megafon">
										<img src="./MineBlaze - Покупка доната, привилегий, ключей_files/megafon.svg" data-method="megafon" style="max-height: 80%" alt="">
									</div>
								</button>
								<button title="Perfect Money" data-method="perfectmoney" class="col-4 rounded-3 btn btn-light p-2 ratio ratio-1x1" style="height: 30%; width: 30%">
									<div class="d-flex flex-column justify-content-center p-2" data-method="perfectmoney">
										<img src="./MineBlaze - Покупка доната, привилегий, ключей_files/perfectmoney.svg" style="max-height: 60%" data-method="perfectmoney" class="my-auto" alt="">
									</div>
								</button>
								<button title="Криптовалюта" data-method="bitcoin" class="col-4 rounded-3 btn btn-light p-2 ratio ratio-1x1" style="height: 30%; width: 30%">
									<div class="d-flex flex-column justify-content-center p-2" data-method="bitcoin">
										<img src="./MineBlaze - Покупка доната, привилегий, ключей_files/bitcoin.svg" style="max-height: 80%;	max-width: 80%;" class="m-auto" data-method="bitcoin" alt="">
									</div>
								</button>
							</div>
						</div>
					</div>
					<!-- <div class="modal-footer">
						<button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Закрыть</button>
					</div> -->
				</div>
			</div>
		</div>

		<!-- Sticky -->
		<div class="mt-auto p-4 text-center" style="color: lightgray">
			Мы никак не относимся к Mojang или Microsoft.
		</div>
		<!-- Yandex.Metrika counter --> <script type="text/javascript"> (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)}; m[i].l=1*new Date(); for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }} k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)}) (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym"); ym(50330080, "init", { clickmap:true, trackLinks:true, accurateTrackBounce:true }); </script> <noscript><div><img src="https://mc.yandex.ru/watch/50330080" style="position:absolute; left:-9999px;" alt="" /></div></noscript> <!-- /Yandex.Metrika counter -->
	

</body></html>
