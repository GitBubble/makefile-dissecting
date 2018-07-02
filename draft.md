  
  suppose we have a file name **Makefile** in project root directory, it has following content.

```
include build/core/main.mk
```

then we will invoke our command to build anything we need. emmm..like

```
make product=mini x86_64
```

to achive our purpose, we need to investigate furthur more on the **make** system

how the programe **make** to think our building target, **make** is like a computer god just like make everything happen.


well, **make** is more like a chief master who cook various gorment as your required.but,first we need to order.


we enter the restaurant, sit on the table, and ready to order our favorite food.

we want eat cruise named "panned apple pie"
```
guest: we want a apple pie panned type
chief: ok, let me write the recipe for `panned apple pie`, here is the recipe
guest: thanks
chief: (run to kitche, writing the following recipe)

   .PHONY: panned_apple_pie
   panned_apple_pie:  apple.o sugar.o pan.o oil.o
   cc -o panned_apple_pie apple.o sugar.o pan.o oil.o
   
```
