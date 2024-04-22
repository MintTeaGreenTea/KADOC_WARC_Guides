# KADOC -- WARC Guides and Tools
This repository is divided into two sections that aim to simplify the process of using WARC (Web ARChival) files for research. Thus, the work published here conceives WARCs as not merely files for archival, but rather as legitimate and useful sources of material for researchers, particularly those interested in digital heritage and culture.

For anyone brand new to Python, I recommend installing [Anaconda](https://www.anaconda.com/download/) and accessing Jupyter Notebooks through it. Once you have opened Jupyter through Anaconda and downloaded the .ipynb files from this repository, open them and run the code--making sure to change the paths to where you have stored your own data. By clicking on each cell and then pressing CTRL + Enter (or clicking on a cell and then clicking "Run" at the top), you will execute the code.
 
 Should you run into any issues or should you have trouble with these notebooks, ***do not hesitate to contact me*** and I'll get back to you as soon as possible!

 ## Tools to Work With WARCs

 These tools focus on extraction for researchers who may wish to work in programs outside of Jupyter and Python. 
 
 ### Text Extraction
 This first notebook extracts the text from the HTML content of each WARC file and saves it as a .txt file. The user has three options:
1- To extract the text from a single WARC file with all its HTML tags (useful if the researcher is interested in the structure of the website).
2- To extract the text from a single WARC file without HTML tags and normalized.
3- To extract the text from a folder of WARC files without HTML tags and normalized. This code returns a single .txt file with the contents of all the websites in the folder.

### Image Extraction
This second notebook extracts all image files from a WARC file and stores them in the user's folder of choice.

 ## Guides to Effectively Use WARCs for Research Purposes
 The contents of this repository aim to provide guides to implement the previously established tools and some new ones to peruse the WARC files and learn from their contents. I have used Belgian Buddhist websites as a case study given my own background in Religious Studies and KADOC's research focus, but these guides should prove useful to any researchers regardless of their primary discipline.
 
 Each of the notebooks are meant to be as accessible as possible for anyone regardless of their level of familiarity with coding and Python, although some experience will help in navigating them. I have annotated what each part of the notebook does and which parameters you should change to fit your own data.
 
 ### Text Analysis Using Warcio
 This first notebook showcases how to use the library Warcio to extract and clean up text, as well as different tools to analyze the text and perform distant reading. It primarily makes use of warcio, spaCy, nltk, pandas, matplotlib, and tkinter. Three different types of visualizations were created for the purpose of better understanding the websites' content. It also creates tkinter window that allows the user to see the frequency of every word in a particular website. 
 
 Some of the visualizations are inspired by those created using the [Voyant-Tools](https://voyant-tools.org/), and given that the first part of the code provides .txt documents, I highly recommend inputing them into the website to gather further information on the content of the WARC files.

 ### Image Analysis
  This notebook exemplifies how to extract images from WARC files to work with them in our Jupyter Notebook. Additionally, it also shows different methods of image analysis available to the user: on the one hand, it makes use of different neural networks to identify elements within the image; on the other hand, it breaks down the images into simpler segments and into their different color values for the user to evaluate. 

 ### Web Network Analysis Using Gephi
_Note that there are several files in the folder for this guide; you'll need to open the .ipynb to access all the code to use on your own WARCs!_ 
  
  This last notebook illustrates how to extract websites from WARC files to create a website network that showcases what each main website most often links to. It also checks what extensions each domain links to so as to understand their positioning in the global sphere. In addition to creating some graphs within the notebook, the code also creates CSV files that can be imported into [Gephi](https://gephi.org/) to generate interactive, cleaner visualizations. 

  
  This portion of the guides requires the highest technical competency if you wish to use Gephi, although you can follow [this guide](https://medium.com/data-analytics-at-nesta/how-to-create-network-visualisations-with-gephi-a-step-by-step-tutorial-e0743c49ec72) from Stage 2 onwards to create your graphs after setting up the nodes.csv and edges.csv file using the code in the notebook. Using Gephi is optional, but you will lose neatness and interactivity if you decide to skip it.

