# Sketch City Hackathon Workshops: Intro to Webscraping with R
## The Iron Yard | Saturday May 6 2017
### Amanda Shih, Neeraj Tandon, Jeff Reichman, Meredith Maines, Randy & a packed house

### Pre-Install Instructions
- download R, install
- download R-Studio, install
- run script: ` source('https://raw.githubusercontent.com/HoustonUseRs/intro-to-web-scraping/master/scripts/setup.r')`

### Approach | Deconstructed
1. Pick a page
2. Load a page
3. Look at page
4. Determine where info is
5. Select info
6. Copy info
7. New file
8. Paste into new file
9. Save new file

### Tool Kit
1. R
2. RStudio
3. Chrome Dev Tools
4. Chrome Selector Gadget Plugin
5. Text Editor


### Getting Started
1. Go to website (www.houstontx.gov/departments.html)
2. Using Selector Gadget, click on the type of data you want. In this case, we want the names of all the people. So, by clicking on one of the names, the chosen name will be green. All other items matching the selector will be yellow. Go through and click on the yellow items that are unwanted, turning them red. Selector Gadget will sort through and figure out the proper/most succinct way to caputre the desired content. In this case, it is `.table150 a:nth-child(1)` 

