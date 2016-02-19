With the schematic almost done it's time to start the board layout. Note that it's hard to get the schematic done before starting the PCB. Let's go trough some steps that I like to do to get it done.

When you start the PCB going from the schematic in eagle you will get all the components and the connections between them. It looks like the mess bellow.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20Organizando%201.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20Organizando%201.png)

The first step is grouping the components in small building blocks, in these case they are easy to identify ( Clock, bottom displays, four displays with decoders and counters, power supply). Use the "ratsnest" command to simplify this 'nest'.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20Organizando%202.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20Organizando%202.png)

Each building blocks has now a lot less connections to the other blocks. The displays driver should be placed near the displays, and the counters for each driver must be near. Placing them on a row seems do make a good fit. The clock divider can stay on the second row, this look's good. The ICs are placed in a order to minimize the leght of the traces, and it's nice they all face the same direction. Take your time to test some diferent configurations in this stage until you think you have a winner.The bottom displays where routed as explained on the design page.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20Organizando%203.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20Organizando%203.png)

Starting routing the PCB, I like to route some power rails first. The routing of the traces on connecting the top IC to each other and the displays traces seems critical. Route this first and remember that you can move things around to get a better routing. I routed the displays segments traces also because there will be four groups routed the same way.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%201.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%201.png)

If you noted i had forgoten the display resistors, so they where added and routed. The bottom part has moved for a better layout. Some of the signals traces where routed, the clock was the first as it must cross all the board.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%202.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%202.png)

Ground plane added on both sides.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%203.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%203.png)

Routing almost complete, some decoupling caps add. Power lines routed with thick traces. Holes for fixind the board in the case also add.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%204.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%204.png)

The board is completely routed. A Design Rule Check (DRC) of the entire board is needed here, both manual and automatically. A good manual check of the board will make the board a lot better to build. The auto DRC will only check if the minimum specs are checked.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%205.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%205.png)

Putting some marks on the board to identify it is a good practice. Since this board will be toner transferred to copper it will not have a silkscreen layer. The marks are then put in both coppers layers.

![http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%206.png](http://74clock.googlecode.com/svn/wiki/images/layout/PCB%20parcial%206.png)

The final step is to print both layers and check them. The components and pads layer also must be printed and the parts placed on the paper to see if the it all fits, and the lead are placed on the pads.

[![](http://74clock.googlecode.com/svn/wiki/images/layout/small/DSC05013.jpg)](http://74clock.googlecode.com/svn/wiki/images/layout/DSC05013.JPG)