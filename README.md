# KADOC -- WARC Guides
 ## Guides to Effectively Use WARCs for Research Purposes
 The contents of this repository aim to provide tools for researchers to use WARC (Web ARChival) files beyond simply accessing and perusing them using tools such as the WayBack Machine. Thus, the work published here conceives WARCs as not merely files for archival, but rather as legitimate and useful sources of material for researchers, particularly those interested in digital heritage and culture.
 
 Each of the notebooks are meant to be easily accessible for anyone regardless of their level of familiarity with coding and Python. I have annotated what each part of the notebook does and which parameters you should change to fit your own data.
 
 For anyone brand new to Python, I recommend installing [Anaconda](https://www.anaconda.com/download/) and accessing Jupyter Notebooks through it. Once you have opened Jupyter through Anaconda and downloaded the .ipynb files from this repository, open them and run the code--making sure to change the paths to where you have stored your own data. By clicking on each cell and then pressing CTRL + Enter (or clicking on a cell and then clicking "Run" at the top), you will execute the code.
 
 Should you run into any issues or should you have trouble with these notebooks, ***do not hesitate to contact me*** and I'll get back to you as soon as possible!

 ### Text Analysis Using Warcio
 This first notebook showcases how to use the library Warcio to extract and clean up text, as well as different tools to analyze the text and perform distant reading. It primarily makes use of warcio, spaCy, nltk, pandas, matplotlib, and tkinter. Three different types of visualizations were created for the purpose of better understanding the websites' content, as well as tkinter window that allows the user to see the frequency of every word in a particular website. 
 
 Some of the visualizations are inspired by those created using the [Voyant-Tools](https://voyant-tools.org/), and given that the first part of the code provides .txt documents, I highly recommend inputing them into the website to gather further information on the content of the WARC files.

 ### Image Analysis
  This notebook exemplifies how to extract images from WARC files, both to save them locally and to simply work with them in our Jupyter Notebook. Additionally, it also shows different methods of image analysis available to the user: on the one hand, it makes use of different neural networks to identify elements within the image; on the other hand, it breaks down the images into simpler segments and into their different color values for the user to evaluate. 

 ### Web Network Analysis Using Gephi
  This last notebook illustrates how to extract websites from WARC files to create a website network that showcases what each main website most often links to. It also checks what extensions each domain links to so as to understand their positioning in the global sphere. In addition to creating some graphs within the notebook, the code also creates CSV files that can be imported into Gephi to generate interactive, cleaner visualizations. 
  This portion of the guides requires the highest technical competency if you wish to use Gephi, although you can follow [this guide](https://medium.com/data-analytics-at-nesta/how-to-create-network-visualisations-with-gephi-a-step-by-step-tutorial-e0743c49ec72) from Stage 2 onwards to create your graphs after setting up the nodes.csv and edges.csv file using the code in the notebook. Using Gephi is optional, but you will lose neatness and interactivity if you decide to skip it.

