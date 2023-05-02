Download Link: https://assignmentchef.com/product/solved-cpsc-51100-statistical-programming-programming-assignment-6-visualizing-acs-pums-data
<br>
<strong>Introduction</strong>

For this assignment, you will work with a survey dataset and use the matplotlib package to visualize data. The data set you will be working with comes from the 2013 American Community Survey (ACS) data. According to census.gov, ACS “is a mandatory, ongoing statistical survey that samples a small percentage of the population every year — giving communities the information they need to plan investments and services.” [see <a href="https://www.census.gov/acs/www/">http://www.census.gov/acs/www/</a>] More specifically, you will be using the ACS Public Use Microdata Sample (PUMS), which census.gov describes as “files [that] are a set of untabulated records about individual people or housing units.”




You can download the 2013 ACS 1-year PUMS data for Illinois Housing Unit Records here:

<a href="https://www.census.gov/acs/www/data_documentation/pums_data/">http://www.census.gov/acs/www/data_documentation/pums_data/</a>




You can also access documentation for the PUMS dataset, including the Data Dictionary, here:

<a href="https://www.census.gov/acs/www/data_documentation/pums_documentation/">http://www.census.gov/acs/www/data_documentation/pums_documentation/</a>










<strong>Requirements</strong>

You are to create a program in Python that performs the following using the matplotlib and pandas packages:

<ol>

 <li>Loads the csv file that contains the PUMS dataset (assume it’s in the current directory) and create a DataFrame object from it.</li>

 <li>Create a figure with 2×2 subplots. The required subplots are as follows:</li>

</ol>

<strong>Upper Left Subplot</strong> – <strong>Pie chart</strong> containing the number of household records for different values of the HHL (household language) attribute. The plot should have no wedge labels, but should have a legend in the upper left corner. The pie needs to be rotated appropriately (see example figure on last page).

<strong>Upper Right Subplot</strong> – <strong>Histogram</strong> of HINCP (household income) <strong>with KDE plot</strong> superimposed. You should use a log scale on the x-axis with log-spaced bins (HINT: use np.logspace).

<strong>Lower Left Subplot</strong> – Bar chart of Thousands of Households for each VEH (vehicles available) value (exclude NaN). Make sure to use the WGTP value to count how many households are represented by each household record and divide the sum by 1000.

<strong>Lower Right Subplot</strong> – <strong>Scatter plot</strong> of TAXP (property taxes) vs. VALP (property value). Make sure to convert TAXP into the appropriate numeric value, using the lower bound of the interval (e.g. 2 -&gt; $1, 16 -&gt; $700, …). Use WGTP as the size of each marker, ‘o’ as the marker type, and MRGP (first mortgage payment) as the color value. Add a colorbar.




<ol start="3">

 <li>Display the figure and save it in a file called ‘pums.png’</li>

</ol>







<strong> </strong>

<strong>Additional Requirements</strong>

<ol>

 <li>The name of your source code file should be py. All your code should be within a single file.</li>

 <li>You need to use the pandas DataFrame object for storing data and matplotlib for visualization.</li>

 <li>Your code should follow good coding practices, including good use of whitespace and use of both inline and block comments.</li>

 <li>You need to use meaningful identifier names that conform to standard naming conventions.</li>

 <li>At the top of each file, you need to put in a block comment with the following information: your name, date, course name, semester, and assignment name.</li>

 <li>The output image file should <strong>exactly</strong> match the sample output shown on the last page.</li>

</ol>







<strong> </strong>

<strong>What to Turn In</strong>

You will turn in the single vispums.py file using BlackBoard.













<strong>Sample Output</strong>




<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/08/166.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/08/166.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>








