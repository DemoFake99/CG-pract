#include <graphics.h>
#include <stdlib.h>
#include <stdio.h>
#include <conio.h>

void main()
{

   int gd = DETECT, gm, errorcode;
   int xmax, ymax, midx, midy;
   initgraph(&gd, &gm, "c:\\turboc3\\bgi");

   xmax = getmaxx();
   ymax = getmaxy();
   midx = xmax / 2;
   midy = ymax / 2;

   line(midx,0,midx,ymax);
   line(0,midy,xmax,midy);
   line(0,0,0,ymax);
   line(0,0,xmax,0);
   line(xmax,0,xmax,ymax);
   line(0,ymax,xmax,ymax);

   getch();
   closegraph();
}