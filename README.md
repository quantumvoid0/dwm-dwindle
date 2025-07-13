# dwm-dwindle
dwindle layout patch for DWM

### Usage
step 1 : download the `dwindle.patch` file from this repo to ur DWM folder

step 2 : `cd` to ur dwm folder and then run `patch -p1 < dwindle.patch`

step 3 : at the top of your `config.h` add `void dwindle(Monitor *m);`

step 4 : in our layout section add dwindle like so :
```c
static const Layout layouts[] = {
	/* symbol     arrange function */
	{ "[]=",      tile },   
	{ "[D]",	  dwindle }, // added dwindle layout
	{ "><>",      NULL },   
};
```
