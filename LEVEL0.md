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
