# Sticker Costing Report

George Pastushok

### Table of Contents

[Introduction](##Introduction)

[Materials](#Materials)

[Costs](#Costs)

[Labor](#Labor)

[Conclusion](#Conclusion)

## Introduction

My goal was to create an analysis and breakdown of what sticker production could cost. I needed to report the following:

- Sticker vinyl cost
- Laminate cost
- Labor cost (est)
- Required time

### Methodology

I started by estimating an average size of stickers based on what I've been printing already. I settled on 3", meaning that the following calculations are based on a 3"x3" square of material for 1 sticker. I grabbed an average size sticker from my stickers folder and set it up for printing. I could fit about 9 stickers across the sheet, which is the minimum order of stickers plus extras. The sheet is set up with about .15" of gap between artworks on a width of about 28.3". The stickers and gaps take up about 28.2" on the sheet width out of a total of 30" on the roll width. I printed the job with crop marks on the entire area, set in the marks tab in the job settings window in VersaWorks. The sheet is set to cut after printing with a 10mm page spacing. The print job is set to print only in the cut controls tab of the job settings. Once all the correct settings have been verified, I set my timer then print the job which takes about 5 minutes. Once the job is printed and comes off the printer I take it to the weeding and masking tables to laminate them. To laminate them, I took the roll of laminate, pulled out a few inches, took a t-square and lined it up 5" from the edge of the laminate and I made a cut. To apply the laminate I peeled a little bit of the backing paper and stuck it down on top of the sticker vinyl. Then with a squeegee I pressed down and ran the squeegee across the laminate to apply it and keep air pockets out. Then the laminated sheet made its way back into the printer for cutting. In VersaWorks, I get the same job, go to the cut settings tab and set it to cut only. With the marks turned on in the settings the printer will try to find the marks on the sheet and set it's alignment for cutting. After the sheet is cut its taken off the printer and stickers are removed from the sheet. Once all the stickers are separated I stopped the timer.

## Materials Costs

### Hardware

I have included the costs for hardware but I have not yet accounted for their costs in the value of a print job yet.

|Item | Cost | Category | Description |
| - | - | - | - |
|[VG2540](https://www.wellingtonhouse.com/p-1987-truevis-vg2-series.aspx)|$22000|printer|new dedicated printer|
|[RSC820CLS](https://www.wellingtonhouse.com/p-1882-rsc-820cls.aspx)|$3900|laminator|32" cold laminator|
|[MPI2903](https://www.wellingtonhouse.com/p-1898-digital-media-sticker-material.aspx)|$147.38|sticker vinyl|the material I'm currently using|
|[MPI3303](https://www.wellingtonhouse.com/p-1898-digital-media-sticker-material.aspx)|$98.25|sticker vinyl|vinyl I could potentially be using|

[DOL2080](https://www.wellingtonhouse.com/p-1898-digital-media-sticker-material.aspx) $172.88 laminate vinyl matte laminate

### Media specs

The materials we use have very similar dimensions, but have different amounts of use.

|media spec | value|
|-|-|
|est. sticker size | 3" |
|lam roll length | 1800" |
|lam roll width | 30" |
|sticker roll length | 1800" |
|sticker roll width | 30"|

With those constants out of the way I can tell you about how much vinyl I use per job:

|media usage type | value |
|-|-|
|vinyl used/job | 11.5" |
|lam used/job | 5"|

Then there is how much I don't use per job:

|media usage type | value|
|-|-|
|sticker spacing |0.15"|
|margins (combined) |2"|

### Media waste

Now I can get into how much exactly isn't used in a print job by taking all these values and converting them into in<sup>2</sup> I need the area of the roll to figure out how much space there is that is potentially usable. The area of

the roll in in<sup>2</sup> is easy to calculate so once I have that I can calculate the area of all other aspects of the print jobs like the sticker (did that earlier), actual job length, margins, gaps and feed margins.

### Print Job

|Formula |Value |Measurement|
| - | - | - |
|VinylUsePerSheet|StickerRollWidth \* vinylUsedPerJob|345 in<sup>2</sup>|
|CombinedStickerSpace|StickerSize2 \* 9|81 in<sup>2</sup>|
|UnusableSpace|VinylUsePerSheet - (CombinedStickerSpace + (StickerSize \* StickerSpacing \* 9) )|259.95 in<sup>2</sup>|
|LaminateUsed|LaminateUsedPerJob \* LaminateRollWidth|150 in<sup>2</sup>|
|LaminateUnused |CombinedStickerSpace - CombinedStickerSpace |69 in<sup>2</sup>|

A side note for the 9 I used in the CombinedStickerSpace, I got that from counting how many stickers at 3" fit across the sheet in VersaWorks. Alternatively it could be calculated by taking the (SheetWidth - Margins) / (StickerWidth + StickerSpacing) then rounded down to the nearest whole number. It would make the formulas in the table very long, so I opted to simplify. With the basic calculations out of the way, I can take the numbers I got in the previous table and use them to calculate costs.

## Costs

To set up the calculations for figuring out the costs for sticker production I need price/in<sup>2</sup> of an entire roll. This is easy as its just Price/(Length\*Width), same goes for the laminate.

|Material |price/in<sup>2</sup>|
|-|-|
|StickerPerSqIn |$0.00273 |
|LaminatePerSqIn | $0.00320|

Now I need to calculate how much cost is associated with a single print job to find out how much it costs to run off as little as one order of stickers(6 stickers). With that I can figure out how much an individual sticker costs by adding StickerVinyl and LaminateVinyl and multiplying the sum by the StickerArea: $0.053 My total materials cost is going to be the sum of the product of *VinylUsedPerSheet and StickerVinylCostPerSqIn* and the product of *LaminateUsedPerSheet and LaminateCostPerSqIn* My total unusable materials cost is going to be the sum of the product of *UnusableSpace and StickerPerSqIn* and the product of *LaminateUnused and LaminatePerSqIn* This Gives me two important numbers to show, I get the approximate cost in dollars of one print job of 9 stickers at 3" with both sticker vinyl and laminate factored in.

|Materials Cost |Unusable|
|-|-|
|$1.11 |$0.69|

## Labor and Machine Time

Now to factor in the cost of labor.

### Breakdown

Since I timed a run of stickers, I have the values all recorded and I can vouch for their feasibility. My timed run of stickers looked like this:

|Checkpoint|Time|Task|
|-|-|-|
|1|  0:00| Print|
|2| 0:05| Cut-off|
|3|  0:07| Dried|
|4|  0:10| Laminated|
|5|  0:11| Reloaded|
|6|  0:15| Cut-off|
|7|  0:17| Popped out|

Steps 1-2 and 5-6 are machine time, which comes out to about 9 minutes. Steps 3-5 and 6-7 are labor time which comes out to 6 minutes Step 2-3 is idle, where the print could either be cut off and moved to the lamination stage, but not be laminated yet or sits on the printer waiting for the laminator to be available. 2 minutes is spent there. Idle time (between 2 and 4, and between 4 and 5) has not really been considered in this timeline, so I would say that 17 minutes is a best case scenario for output speed. Stickers of different proportions and outline shapes will affect how much time is required to cut. Simple shapes are faster and more intricate cut lines will take more time. I have an estimate for the cost of labor while making the assumption that the Printer earns $22/hr and the Assembler earns $19/hr

|Task|Minutes|Role|Cost|
| - | - | - | - |
|Queuing for printing|1|Printer|$0.37|
|Removing from printer|1|Printer|$0.37|
|Laminating|3|Assembler|$0.95|
|Loading printer|1|Printer|$0.37|
|Separating and Packing|3|Printer|$1.10|
|-|-|**Total**|$3.15|

Alternatively the separating and packing step could be completed by an Assembler for a reduction to $0.95 for that step, $3.00 for the process.

## Conclusion

I think the process is pretty streamlined from my tests. There are a few spots where we could run in to some issues in the future with quality and efficiency. I am still looking in to Laminating machines and maybe a dedicated printer and dedicated cutter. Those add additional costs I have not factored in like depreciation and maintenance. My reasoning for using 1 print job for finding the cost rather than a single sticker is because I think that is a more realistic way of looking at how much material will be used and unused. If I were to print just 6 stickers the wasted material would be much higher relative to the amount of material used. So I think printing stickers in batches with extras for use later will be much more cost effective and speed up the process next time an order comes through as well as creating extras in the case that something goes wrong with a sticker in the production process.

In the long term I need to calculate the loss from production errors that may come up so we can factor that in to our costs.

### Costs Summary

|key |value |
|-|-|
|StickerJobs/Roll |157 |
|Stickers/Roll| 1409 |
|Cost/Roll| $666.46 |
|Stickers/Order| 6 |
|Revenue| $10 |
|Profit| $7.16 |
|ProfitMargin| 72%|
