# Evil-Bookmarklet
A Bookmarklet that converts all your text to, “2.2 when?” As you type. Useful if you want to spam RobTop but don’t actually want to take the time to type it out.
# Download

[2.2 When?](javascript:(function()%7B(function()%7Bvar%20TEXT%20%3D%20'2.2%20when%3F%20'%3BArray.prototype.slice.call(document.querySelectorAll('input%5Btype%3Dtext%5D%2Ctextarea')).map(function(el)%7Bel.onkeypress%3Dfunction(evt)%7Bvar%20charCode%20%3D%20typeof%20evt.which%20%3D%3D%20%22number%22%20%3F%20evt.which%20%3A%20evt.keyCode%3Bif%20(charCode%20%26%26%20charCode%20%3E%2031)%20%7Bvar%20start%20%3D%20this.selectionStart%2C%20end%20%3D%20this.selectionEnd%3Bthis.value%20%3D%20this.value.slice(0%2C%20start)%20%2B%20TEXT%5Bstart%20%25%20TEXT.length%5D%20%2B%20this.value.slice(end)%3Bthis.selectionStart%20%3D%20this.selectionEnd%20%3D%20start%20%2B%201%3B%7Dreturn%20false%3B%7D%7D)%3B%7D())%7D)())
