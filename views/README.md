# Performance of main.js

Reduced from
![Main.js OLD](js/performance_main_old.PNG)

TO
![Main.js NEW](js/performance_main_new_minified.PNG)

The most important increase of performance is due to:

	if(pizzaTop > innerHeight) {
      break;
    }

at the bottom of the main.js class. With it we only create as much pizzas as the ones that can be visible.