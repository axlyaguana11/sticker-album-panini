# How many sticker packages should I open to fully complete Panini's World Cup Album?

In this repo, I simulate 1000 times the opening of packages with Panini's World Cup Album 2022. 

## Methodology and considerations

I considered the following:

* Each sticker is randomly assigned to a package.
* The sampling is with replacement. So that, we have duplicates.
* Basically, this is a bootstrapping approach.

Album and packages features:

* To complete the album, you should collect 638 different stickers.
* There are other 80 additional stickers. They are not part of the main collection. So I didn't considered them here.
* Each package comes with 5 stickers inside.
* The price of each package varies from country to country. In my case (Ecuador) it's 0.80 USD.

## Results

After simulating 1000 times, we get a distribution as follows:

![](https://github.com/axlyaguana11/sticker-album-panini/blob/main/figures/figure_1.png)

And the cumulative probability:

![](https://github.com/axlyaguana11/sticker-album-panini/blob/main/figures/figure_2.png)

From those figures, we can summirise numerically as follows:

                 
count  1000.000000
mean    902.181000
std     163.262828
min     572.000000
25%     792.000000
50%     873.000000
75%     984.250000
max    1693.000000

Having a CI at 95%: 659.975, 1307.300

## Conclusions and recommendations

* The number of packages you should open is between 660 and 1307 (95% CI).

* You need a minimum of 572 packages, but the probability of completing the album with those is very low. Less than 1%.

* In order to get a probability of 90% of completing the album, you need at least 1108 packages.

* There may be a different and optimal approach of completing the album. We can find a number of packages where we can start buying stickers individually. Of course each sticker sold individually is more expensive, but I encourage you to figure out whether it's a better approach. 

## References 

[FIFA World Cup Qatar 2022™ - Box of 50 sticker packets |Panini](https://www.paninistore.com/shp_int_en/fifa-world-cup-qatar-2022-box-of-50-sticker-packets-panini-bundle004286b5bexp1-it.html)

[FIFA World Cup Qatar 2022™ - Hardcover Sticker Album |Panini](https://www.paninistore.com/shp_int_en/fifa-world-cup-qatar-2022-hardcover-sticker-album-panini-004286aexpinth-it.html)

[What the Euro 2020 Panini sticker album can teach us about probability](https://theconversation.com/what-the-euro-2020-panini-sticker-album-can-teach-us-about-probability-160797)