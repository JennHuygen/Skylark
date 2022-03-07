Understanding Roof Shapes
=======================================================

According to the [WikiHouse Skylark design guide](https://www.wikihouse.cc/guides/design#roofshape), there are different roof sizes you can consider:

1.  Flat or parapet roof — the first is an actual flat roof designed with a slight angle for rainwater drainage, the second uses the floor beams to create a completely flat roof which can be helpful for terraces
2.  Sloping roof — one side is higher than the other and it creates additional internal height
3.  Gable roof — a traditional triangle-shaped roof

As last week’s Skylark update included walls that fit with the gable roof, this was an excellent time to start modelling the different types of roofs in SketchUp to understand not only what the roofs would look like, but also how you can model them using Skylark blocks.

However, I quickly noticed that not all roof blocks are available yet:

-   The flat roof blocks are supposed to be pre-engineered with a 1:80 slope to allow rainwater to run off. However, they are not currently in the Skylark blocks library so the only flat roof type you can create is the parapet roof for terraces (or to later build a second storey on your house).
-   The sloping roof isn’t available yet either. While you can create the wall structure for it by modelling a M-sized wall on one end and a XL-sized wall on the other, there are no roof COMBS or blocks to connect the walls. Using the Gable-roof combs didn’t help either because the sloping roof is supposed to come pre-engineered with a 10 degree pitch.

In addition, I also learned that to create the roof, you need to use a third type of COMBS. There are two types of combs that I used before — A or B and you use them for the ground or mid-level floors respectively. However, to create the roof, you need to use the COMB_G for the Y-axis. These combs **are** included in the starter kit that you can download from the WikiHouse website, but they **are not yet** mentioned on the blocks library. Similarly, the end verge for the gable roof **is** included in the starter kit, but **is not yet** listed on the WikiHouse website in the blocks library.

Here is how all this looks like in SketchUp and the steps I took to practice with the Skylark blocks.

### Creating a gable roof

_House frame_

To create the frame of the house, I used two of the MEDIUM_B_X blocks that I created myself as part of a redesigned starter simple designer kit. These blocks already have the X-level combs and the end floor block fitted on to them so I only need to pay attention to how long I want the Y-axis to be.

I created the Y-axis using the COMB_A_END_Y1 and Y2 for the ends with COMB_A_MID_Y in the middle. I then reversed the order to create a second comb line for the Y-axis, aligned it with the first line I created, and grouped it to have a double line Y-axis. I then slipped them into the X-axis connections on the front and the back. Then I copied the Y-axis group, turned them 180 degrees, and slipped them into the X-axis on the other side of the house.

I then added eight FLOOR_M blocks to create the floor of the house. Finally I added four CORNER_M posts in each corner of the frame, making sure to turn them 95 degrees each time to make them fit exactly into the floor ends.

_Gable roof_

To create the gable roof, there are different X and Y-axis combs to consider. First I modelled the Y-axis combs as there is only one type of X-axis comb that fits, which is the COMB_G_END_X1.

For the Y-axis, I used the same structure as for the ground floor combs, but this time I used the COMB_G combs instead of the COMB_A combs. The G referring to this being applicable for the gable roof. So that meant I used the COMB_G_END_X1 and X2 for the ends and the COMB_G_MID_X for the middle. As I mentioned at the start, these blocks are included in the full design kit when you download it from the WikiHouse website, but are not listed under the blocks library on the website.

So to create the Y-axis you repeat the same steps as for the ground floor: once you have connected one row, reverse them for the second row, align them face to face, and group them together. Then fit them on top of the two end floor blocks on one side of the house. Copy the group and repeat on the other side of the house.

Now you need to add the COMB_G_END_X1. Here it was important to remember that every time you work with combs, you do so in a double layer (the two rows). So what I did here was copy the COMB_G_END_X1 and align the two copies with one another, face to face. Then I grouped them so I couldn’t accidentally move them again. Then I did the same for the mid-level of the gable roof x-axis, which is COMB_G_MID_X1. I copied it, aligned it face to face, and grouped the two rows together. Then I aligned the group of mid-combs on to the top of the group of end-combs to create one half of the roof arch. I then grouped the two groups so I couldn’t accidentally move the two parts of the arch out of place anymore.

With the arch grouped, I then made three copies, and slid each copy on top of each end of the Y-axis (all four corners). Note that you will need to turn two of the arch comb groups 180 degrees to make it fit on the other side.

You will now have two gable roof arches made up solely out of combs. This will need to be covered by an actual roof block. The structure for the roof works the same as the floor — that means you add and END roof block on both ends of your home (the outer X-axis), and fill the middle of your build with regular roof blocks (or windows — though the skylight windows are not included in the blocks library yet, despite being mentioned in the design guide). For the gable roof, the block you will need to use is VERGE_G (as noted in the introduction, this block is included in the design kit, but not currently listed in the library on the WikiHouse website).

So what I did was move the VERGE_G on top of my arch combs on the X-axis. I then grouped one of them to create a new component, so I created a new component that has the X-axis combs and verge combined for the gable roof. I updated my starter simple design kit with this so it will be easier in the future to start modelling with the roof right away.

With the combs and verge now in place, all that is left to do is to use the ROOF_G blocks on both sides to fill in the gaps between the two ends of your build. So finally, your gable roof will look like this:

[](images/gabled_roof.png)

### Creating a flat roof

While I wasn’t able to create a parapet roof due to the flat roof blocks not yet being available, I tried to model the gable roof and flat roof together to see what a terrace would look like. I copied the model I created for the gable roof, as explained above, and removed the outer VERGE and three rows of roof blocks. This is what it looked like:

![](gabled_roof_terrace.png)

Of course, this isn’t a very realistic model because there is no way now to access the terrace, but it was interesting nonetheless to see the possibilities of adding a terrace as part of the house. We can figure out later how to add stairs in effectively (and once those blocks become available).

I also took this opportunity to practice with the new gable roof walls that were released last week to understand how you would model with them. That really couldn’t have been simpler. There are four types of gable roof walls, and you use them in order so that the walls align with the gable roof. These are the WALL G1, G2, G3 and G4 blocks. You start with G1 in the corner of your build on the X-axis, then next to that goes G2, then G3, and then G4. This is how it looks like:

![](gabled_roof_walls_png)

This does imply, however, that you cannot have any windows or doors on the X-axis where you are using the gable walls. Which makes sense from a structural point-of-view, but from a home-point-of-view you would like want to then add a skylight window (once available) to allow more daylight to fall in.

### Creating a sloping roof

Finally, I also practiced the sloping roof form. I used the same foundation as the gabled roof build, but replaced one side of the corner walls with the XL corners. Unfortunately, as I mentioned at the beginning, the special combs and roof for the sloping roof with the 10 degree angle isn’t available yet. However, by modeling the different walls and putting a COMB_G_END_X1 on either end, you can almost see what it is supposed to look like:

![](sloped_roof_incomplete.png)

#### A final note

In all my roof practice designs I have used the layout of a simple one level house. If you would use a two floor house, for example, you would need to model differently by using the mid-level combs when you are creating your second floor, as explained in my other practice models. It also means that your house will become quite high if you are building two floors, as the gable roof needs to have the M-level walls but at its highest point the wall is 4.7m. In that way you could create an attic, I think, as part of your second floor. But if you don’t want an attic, it may makes more sense to wait until the sloping roof design is available.

My next step will be to model a more detailed house with the gable roof and some room layouts included so I will test that reflection in the next few weeks.