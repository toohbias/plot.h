# plot.h
A very simple, memory efficient (and badly written) plotting library for c
## FEATURES
- simple Plots without the need to store all values in (huge) arrays and having to iterate over them again to plot them
- title/axis labelling
- automatic axis scaling
- saving Plots as compact .pbm image
- segfault proof (hopefully)
- all conveniently inside a single header
## USAGE
**Initialising a Plot:**

```
Plot p = initPlot(double x_min, double x_max, double y_min, double y_max, char *x_label, char *y_label, char *title, char *file_name);
```
**Plotting a Point:**

```
setPoint(double x, double y, Plot *p);
```
**Saving a Plot:**

```
savePlot(Plot *p);
```
**Changing the resolution:**

You can change the ```#define WIDTH``` and ```#define HEIGHT``` at the top of the header.

Note that the width should be a multiple of 8.
## EXAMPLE
![](https://github.com/user-attachments/assets/601c2c14-41d9-436c-b8f6-4868a7a0caaa)
