# datasci_4_web_viz
HHA 507 HW 4

**1. R's Shiny Visualization:**
* This is my [Shiny App R](https://ba0tb1-megan-le.shinyapps.io/RShiny_Texas/)
![image](https://github.com/meglee67/datasci_4_web_viz/assets/123908362/b006c98c-5c2b-46e8-956c-2fbeeb78a078)

* The challenge I encountered in this deployment was that I didn't realize that you could write directly in the console within Postit Cloud. Once I figured out that was possible, then I just followed the steps listed in the [deployment directions](https://docs.posit.co/shinyapps.io/getting-started.html#working-with-shiny-for-python) and was able to successfully connect my shinyapps.io account, click down the publish options menu, select that I wanted to publish my app to the shinyapp.io account and not the postit cloud.
* Alternatively if you don't want to connect your account through the console you can do this
  1. Open posit cloud and open an Rworkspace
  2. Go to the tools tab, click on it and navigate down the dropdown menu to "Global Options"
  3. In the menu that pops up, on the lefthand side, click 'Publishing"
  4. Click the button that says "connect" and choose to connect your account to ShinyApps.io and then do the token copy and paste to connect your account
* Also I had trouble with the initial dataset I chose (Florida) so I went back to the [CDC website](https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-County-Data-20/swc5-untb) and extracted a new dataset (Texas) and that ended up working.

**2. Python's Shiny Visualization:**
* I went through many struggles during this stage. First I made sure to pip install shiny and matplotlib. Then once I took the example code and tried to run it via python app.py or shiny run app.py --reload but I got the error that "ImportError: cannot import name 'app' from partially initialized module 'market' (most likely due to a circular import)"
* Then once I took my app.py outside of the shiny_python folder, it ran and created a pycache folder and doing this would work and create a temporary link
* ![image](https://github.com/meglee67/datasci_4_web_viz/assets/123908362/7e705f7c-eef4-4081-85c6-8e85e6afa292)
* I then followed the instructions through this [link](https://medium.com/trevor-french/creating-deploying-shiny-apps-in-python-f446557f6084) in an attempt to push to shinyapps.io and create a permanent link, but ran into the issue of "Error: Nickname does not exist". 

**3. Flask with Matplotlib Visualization:**
* I was unable to get this link to run as it kept telling me the file path didn't exist. Doing this assignment alongside a classmate, we found that if we had other existing .py files, then moving onto the next section and trying to run a different .py file it wouldn't recognize or let us.
