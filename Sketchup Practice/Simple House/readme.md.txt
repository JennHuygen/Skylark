# Simple House

Using the updated Starter Simple Design Kit for Skylark 250 that I created, I started practicing by modeling a medium-sized house. The instructions of which are below.

I will likely build on the initial draft I created in the next few weeks so watch this space if you are interested. 

## Create the frame of the ground level floor

Starting with the new component I created that gives you the medium-sized basic end block for the x-axis (MEDIUM_A_X), the width of the practice house was easily determined. 

I then decided how long the Y-axis will need to be. I decided to go for eight spaces between the end walls -- that means there are eight double peaks on the Y-axis combs, flanked by an individual peak on either end where the Y-axis means the X-axis.

To create the Y-axis I used the following combs:

 - COMB A END Y1
 - COMB A MID1
 - COMB A END Y3

I then reversed that order to create a second row face to face of the first row. That is one side of the Y-axis done which you can slide into the end of the X-axis. I grouped those two rows for the Y-axis together, copied them (M key, CTRL in SketchUp), and moved the copy to the other end of the X-axis. Sliding the copied Y-axis into the other end of the X-axis. This will then give you a U-shape.

Then finally you will need to copy the MEDIUM_A_X and move it to the open end of the U-shape to finish the frame of the ground level floor. Here I noticed I had to rotate the component 180 degrees to slide it nicely into both Y-axis ends. 

## Adding floors

Now that you have the outline of the house, adding floors is simple. Use the medium-sized basic floor beam (FLOOR M block) and place it on the inside of either end floor block. Copy eight times to fill in the floor (easiest way to do this in SketchUp is to copy the first floor beam, place it right next to the first floor beam and, without clicking anywhere else, type 'x7' so that SketchUp will fill this in automatically for you).

## Adding walls, windows and doors

Start by placing a medium-sized corner post (CORNER M) in each of the four corners of the house. Note that you will need to rotate the corner post 95 degrees each time to make the cutouts slide nicely on top of the floor ends.

Once you have put all the corner posts in, you can add in the walls, windows and a door. The model house I created has a large window at the back of the house, two windows on each side of the house, and two windows and a door at the front of the house. **Note that I do not know if this is structurally sound but this is still a practice after all.**

Starting with the front of the house, I added:

 - Two medium-sized window blocks (WINDOW M1) on the left.
 - Two basic wall blocks (WALL M) on the right side of the windows.
 - One medium-sized door block (DOOR M1).

Make sure you rotate the wall, window and door blocks 180 degrees if needed so that the inside (where the small cutouts are) is facing the inside of the house.

Starting from the front of the house and moving towards the back of the house, I added on both Y-axis:

 - Two basic wall blocks (WALL M).
 - One medium-sized window blocks (WINDOW M1).
 - Two basic wall blocks (WALL M).
 - One medium-sized window blocks (WINDOW M1).
 - One basic wall block (WALL M).

Again, make sure that the wall and windows are rotated correctly.

Finally, I added in the back walls and windows of the house on the remaining free X-axis:

 - One basic wall block (WALL M).
 - Three medium-sized window blocks (WINDOW M1).
 - One basic wall block (WALL M).

Again, make sure that the wall and windows are rotated correctly.

## Creating the mid-level frame

To be able to add the roof (or the second level of the house depending on what you are building), you will need to use COMBS again to connect the walls with the floors/roof on the mid-level.

For this, I repeated the same steps as for the ground level floor, but the only difference is that this time I used the B COMBS, which are the mid-level combs. This means I used:

 - Two times MEDIUM_A_X for the X-axis
 - Two times a combination of two reversed rows of COMB B END Y1+COMB B MID1+COMB B END Y3 for the Y-axis

Make sure the corners of the X-axis and the Y-axis slide neatly into one another.

## Adding a simple roof

As there are no flat roof blocks available yet in the Skylark library, repeat the steps for 'adding floors' but this time on the mid-level of your build so you can create a simple roof.
