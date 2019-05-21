# Fingerprinting Browser

Fingerprinting browser with JS

## It uses:
1. jQuery
2. JS SHA Lib
3. Fingerprint2js

## Useage:
Import the js libraries into html file as usual. JS libraries are provided in the src folder
Paste the code given below and the input box with name='fp' will contain the fingerprint

## Code:

    <script src="src/jssha3.js" async></script>
	<script src="src/fp2.min.js"></script><input type='hidden' name='fp'>
	<script>
	window.onload=function(){Fingerprint2.get(function(e){document.getElementsByName('fp')[0].value=sha3_256(e.map(function(e)		{return e.value}).join())})}
	</script>

#### Use:
	var fp = $('[name=fp]').val();

## Other info:
In Django and Flask there is a library to do the same (Search for pip install bfa) https://pypi.org/project/bfa/
