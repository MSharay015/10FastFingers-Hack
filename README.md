# 10FastFingers-Hack

Copy-paste this in your browser console to get maximal words per minute -> https://10fastfingers.com/typing-test/english

var input = $('#inputfield')[0]
var ev = $.Event('keyup')
ev.which = 32
setInterval(function() {
    if ($('.highlight')[0]) {
        input.focus()
        input.value = $('.highlight').text()
        $(input).trigger(ev)
    }
}, 100)
