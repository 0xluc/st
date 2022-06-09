# My suckless utilities configuration 
Inspired by [Hex Dsl](https://www.youtube.com/watch?v=UEmPboaTDpQ)

## How it works?
Each patch and my main configuration are in separate branches as the master is the default configuration, to aply it all you must merge it all into the master branch

## How make a new patch?

```bash
patch -p1 < 0001-whatever.patch
make && sudo make clean install ## make a new binary
make clean && rm -f config.h && git reset --hard origin/master # returns to starting point
```