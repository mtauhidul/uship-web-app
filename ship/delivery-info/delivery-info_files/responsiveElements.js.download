jQuery.support.placeholder = (function () {
	var i = document.createElement('input');
	return 'placeholder' in i;
})();

var handlePlaceholderText = function(isResponsive, exampleTextSelector) {	
	hPT = {};
	hPT.isResponsive = isResponsive;
	hPT.windowWidth = window.innerWidth || window.document.documentElement.clientWidth || window.document.body.clientWidth || 0;
	hPT.exampleTextSelector = exampleTextSelector;
	hPT.formExampleText = $$(exampleTextSelector);

	function init() {
		if (hPT.formExampleText) {// && hPT.isResponsive === 'true' && hPT.windowWidth < 768
			if (jQuery.support.placeholder) {
				for (var i = 0; i < hPT.formExampleText.length; i++) {
					$(hPT.formExampleText[i]).setStyle("display:none;");
				}
			}
		}	
	}
	
	init();
	return hPT;
};
 