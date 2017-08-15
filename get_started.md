---
title: Get Started
layout: get_started_landing
description: Sign up today to step away from the charts. All we need to get you started is your phone number.
---

<!-- Main -->
<div id="main">

<script type="text/javascript">
  /* <![CDATA[ */
  goog_snippet_vars = function() {
    var w = window;
    w.google_conversion_id = 1017746846;
    w.google_conversion_label = "0xIRCN_46XIQnqum5QM";
    w.google_remarketing_only = false;
  }
  // DO NOT CHANGE THE CODE BELOW.
  goog_report_conversion = function(url) {
    goog_snippet_vars();
    window.google_conversion_format = "3";
    var opt = new Object();
    opt.onload_callback = function() {
    if (typeof(url) != 'undefined') {
      window.location = url;
    }
  }
  var conv_handler = window['google_trackConversion'];
  if (typeof(conv_handler) == 'function') {
    conv_handler(opt);
  }
}
/* ]]> */
</script>
<script type="text/javascript"
  src="//www.googleadservices.com/pagead/conversion_async.js">
</script>


<script>
	goog_report_conversion();
	function onPhoneFormSubmit(token) {
    document.getElementById("phoneForm").submit();
  }
</script>

<!-- Three -->
<section id="three">
	<div class="inner">
		<header class="major">
			<h2 class="accent">Join CrypTck</h2>
		</header>
			<form action="https://api.cryptck.com/production/web/inbound" method="POST" id="phoneForm">
        <div class="field half first">
          <label for="number">Enter your US phone number</label>
          <input type="tel" name="number" id="number">
        </div><br><br>

        <div class="field half first">
          <label for="cryptocurrencies">Select the CryptoCurrencies you'd like to track:</label>
          <div>
            <span class="crypto-radio">BTC Bitcoin</span>
            <span class="crypto-radio">ETC Ethereum</span>
            <span class="crypto-radio">LTCLitecoin</span>
          </div>
        </div><br><br>

        <div class="field half first">
          <label for="currency">Which currency would you like to track with?</label>
          <div>
            <input type="radio" name="currency"> &#36; US Dollars<br>
            <input type="radio" name="currency">&euro; Euros<br>
          </div>
        </div><br><br>

        <div class="field half first">
          <label for="interval">Set your alert interval ranges:</label>
          <p class="helper-text"><i>e.g., if you would like to receive an alert when the price of ETH moves up or down by &#36;50, set the ETH interval slider to '50'</i></p>

          <!--BTC Slider-->
            <div class="range-slider">
              <span class="accent">BTC:</span>
              <input class="range-slider__range" type="range" min="1" max="1500">
              <span class="range-slider__value">1</span>
            </div>

            <!--ETH Slider-->
              <div class="range-slider">
                <span class="accent">ETH:</span>
                <input class="range-slider__range" type="range" min="1" max="1000">
                <span class="range-slider__value">1</span>
              </div>

              <!--LTC Slider-->
                <div class="range-slider">
                  <span class="accent">LTC:</span>
                  <input class="range-slider__range" type="range" min="1" max="500">
                  <span class="range-slider__value">1</span>
                </div>

        </div><br><br>

					<ul class="actions">
						<li>By clicking "Start" you agree with our <a href="https://cryptck.com/terms.html" target="_blank">Terms and Conditions</a>.</li><br><br>
						<li>
						<button
						class="primary special g-recaptcha"
						data-sitekey="6Lc59yMUAAAAAJiwYDYK7BPx3RHsD5dTEdF2xe9f"
						data-callback="onPhoneFormSubmit">
						Start
						</button>
						</li>
        	</ul>
      </form>
	</div>
</section>

</div>
