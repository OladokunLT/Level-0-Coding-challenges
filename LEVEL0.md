// Task 0.1 addition

    x = 0;
    y = 1;
    console.log(x);
    console.log(y);
    x = x + 3;
    y = y + x;
    console.log(x);
    console.log(y);

//Task 0.2 Bodmas

    x = 1 + 1 * 2;
    y = (1 + 1) * 2;
    z = 1 + ( 1 * 2 );
    a = 1 + 1 * 2 / 2;
    b = (1 + 1 * 2 ) /  2;
    console.log(x);
    console.log(y);
    console.log(z);
    console.log(a);
    console.log(b);

// Task 0.3 Greeting

    function hello(name) {
        var greeting = "Hello " + name + "!"; 
        console.log(greeting);
    }
    hello("Tshepo");

// Task 0.4 Even or Odd figure
	
    function evenOrOdd(val){
   	if (val % 2 == 0){
            console.log("even");
        } else {
            console.log("odd");
        }
    }
    evenOrOdd(3);

// Task 0.5 Area of triangle with three sides

    function areaOfTriangle(x, y, z)  {
        var s = (1/2) * (x + y + z);
        var area = Math.sqrt(s * (s-x) * (s-y) * (s-z));
        console.log(area);
    }
    areaOfTriangle(3, 4, 5);

//Task 0.6 Maximum figure

    function maximum(...y) {
    	var a = 0;
    	var c = y;
    	for (var val of c){
            if (val > a){
                a = val;
            }
    	}    
    	console.log (a);
    }
    maximun(4, 3, 9);

 
//Task 0.7 Temperature conversion

	function celciusToFarh(val){
	    var answer = (val*9/5) + 32
	    console.log(answer);
	}
	centToFarh(0);

	function farhneitToCelcius(val){
	    var celcius = 5/9 * (val - 32);
	    console.log(celcius)
	}
	farhneitToCelcius(98.6);


// Task 0.8 Hour and Minute.

	function hourAndMinute(params) {
	    var x = parseInt(params / 60);
	    var y = params % 60;
	    var hr = x + " hour"
	    var min = y + " minute"
	    if (x > 1) {
	        hr += "s"
	    } else if (y > 1) {
	        min += "s"
	    } else if (!x) {
	        hr = '';
	    }
	    console.log(hr +  ", " + min)
	}
	 hourAndMinute(146);

// Task 0.9 extract unique vowels in string.

	function vowel(param){
	    param = param.toLowerCase();
	    var arr = ["a", "e", "i", "o", "u"];
	    var put = [];
	    for (let i=0; i < param.length;  i++) {
	        for (a of arr) {
	            if (param[i] == a) {
	                put.push(a);
	            }
	        }
	    }
	    put = unique(put)
	    return put;
	}
	function unique(param) {
	    arr = []
	    for (let i = 0; i < param.length; i++) {
	        if (arr.indexOf(param[i]) !== arr.lastIndexOf(arr[i])) {
	            continue;
	        }
	        arr.push(param[i]);
	    }
	    return arr;
	}
	console.log(vowel("Umuzi"));


// Task 1.0 Common letters of two strings

	function commonLetters(string1, string2) {
	    var arr = [];
	    for (var s1 of string1) {
	        for (const s2 of string2) {
	            if(s1 == s2){
	                arr.push(s1)
	            }
	        }
	    }
	    arr = unique(arr);
	    return arr;
	}
	var val = commonLetters("oladokun", "lukman");
	console.log (val)
