# ExportDesmosData
There is no built-in way you can export the data points that you graph on the desmos.com/calculator.com web-app. This is a simple set of steps for extracting, cleaning and transforming the data points from the desmos graphing calculator web-app.

Step 1: 

After you have plotted your graph, open up the chrome console and type the command:
  
  document.querySelector("#graph-container > div > div > div > div:nth-child(1) > div > div.dcg-exppanel-container.dcg-add-shadow > div.dcg-exppanel.dcg-disable-horizontal-scroll-to-cursor > div > span > div.dcg-expressionitem.dcg-expressiontable.dcg-selected > div.dcg-fade-container.dcg-disable-horizontal-scroll-to-cursor > div > div > div").innerText
  
--This outputs the rows and columns in which the x and y values of your graph are stored

Step 2:

  Copy the output to a text file
  
Step 3:

  Run the plots_clean.py script from the same directory in which the above text file is saved
  
That's it! Now you have the plots in an easier to manage format.
