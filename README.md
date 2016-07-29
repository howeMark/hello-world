# hello-world
# a short description
# a bit about yourself


# js

var mark = { 
	form : 'human',
	name : 'Mark',
	alignment : 'chaotic neutral'
	}

function reverseStr(s) {
  for (var i = s.length - 1, o = ''; i >= 0; o += s[i--]) { }
  return o;
}


function transmogrifier(mark) {
	if (typeof mark !== 'object') { 
		console.log('input is of the wrong type'); 
		return;
	}
	
	// generate a random number between 1 and 5
	
	var randomNum = Math.floor(Math.random() * 5) + 1;
	
	switch(randomNum) {
		case 1  : mark.form = 'alien', mark.name = reverseStr(mark.name); break;
		case 2  : mark.form = 'crocodile', mark.alignment = 'lawful evil'; break;
  		case 3  : mark.form = 'snek', mark.name = 'Slither' + mark.name; break;
  		case 4  : mark.form = 'Steve Aoki', mark.name = 'dimmakmark', mark.alignment = 'chaotic good' ; break;
  		default : break;
	}
}
