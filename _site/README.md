# P1GFX.github.io

This website is a portfolio of my work as digital artist. I started with the [Artist Theme](https://github.com/DevTips/Artists-Theme) from DevTips and [Travis Neilson](http://travisneilson.com/). I made some modifications - preferring to have a second landing page for projects and to leave off clients for now. The slider that Travis set up for work products is pretty neat, and I'm hoping to find a good place for it later.

Some features that I added:
+ I implemented a twittercard setup that can be unique to each page but defaults to site information if the page information is not available. The meat of that is in `/_includes/twittercard.html` which can just be included into the site head in the index or other stand alone files. For this site, I have included it in the head for index.html and default.html (layout).
+ I created an automatic internal linking system on the `100DaysOfArt.md` page using `daylist.html` - basically, there is a loop in daylist from 0 to whatever number is indicated complete in the YAML for the page and uses the automatic h2 level internal page links from [kramdown](https://kramdown.gettalong.org/syntax.html). It is definitely worth it to read the documentation.
