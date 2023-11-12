<h1>Bigfoot-Sightings</h1>
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="">Business Understanding</a>
      <ul>
        <li><a href="">Scope</a></li>
      </ul>
    </li>
    <li>
      <a href="">Data Understanding</a>
      <ul>
        <li><a href="">Data Source</a></li>
        <li><a href="">Variables of Interest</a></li>
        <li><a href="">Data Types</a></li>
        <li><a href="">Visualisation Requirments</a></li>
        <li><a href="">Comparative Analysis</a></li>
        <li><a href="">Potential Biases</a></li>
      </ul>
    </li>
    <li>
      <a href="">Approach</a>
    </li>
    <li>
      <a href="">Visualisations</a>
    </li>
    <li>
      <a href="">Interpretations</a>
    </li>
    <li>
      <a href="">Technologies</a>
    </li>
    <li>
      <a href="">Setup</a>
    </li>
    <li>
      <a href="">Status</a>
    </li>
    <li>
      <a href="">Credits</a>
    </li>
  </ol>
</details>
<P>The main goal of this project is to answer the questions "Which state within the USA had the most sightings over the period?" and "Within this state which county was responsible for the majority of these sightings?".</P>

<h2>Business Understanding</h2>

<h3>Scope</h3>
<p>This analysis takes place between 1950 and 2018 within the geographical location of the USA.</p>

**Credibility Criteria**  
<p> The Bigfoot sightings were classified into 3 report types:

Class A - These reports involve clear sightings in circumstances where misinterpretation or misidentification of other animals can be ruled out with greater confidence e.g. there are several footprint cases that are very well documented.

Class B - These reports involve incidents where a possible sighting was observed at a great distance or in poor lighting conditions e.g. a report where nothing was seen but distinct and characteristic sounds of sasquatches were heard.

Class C - These reports have a high potential for inaccuracy e.g. most second-hand reports, and any third-hand reports, or stories with an untraceable source. </p> 

<p> In this analysis I consider sightings to be credible if they are within Classes A & B </p>

<H2>Data Understanding</H2>
<h3>Data source</h3>
<p>The data source I am using is the Bigfoot_cleaned Excel file which I obtained through my Introduction to Tableau module in my Data Analytics Essentials course.

I believe this data to be reliable/unreliable because...
</p>

<h3>Variables of Interest</h3>
<p> The key variables I want to analyse within this project are as follows:
<ol>
  <li>Number of sightings</li>
  <li>States in which sightings occured</li>
  <li>Counties in which sightings occured</li>
</ol>
</p>

<h3>Data Types</h3>
<p>My data contains:
  <ul>
    <li>Report Type - String</li>
    <li>Report Class - String</li>
    <li>Submitted Date - Date and Time</li>
    <li>Year - String</li>
    <li>Season - String</li>
    <li>Month - Date and Time</li>
    <li>State - String</li>
    <li>County - String</li>
  </ul>
</p>

<h3>Visualisation Requirements</h3> 
<p>I want to first use a horizontal bar chart in order to visualise the state with the most sightings. Then I want to use a symbol map in order to visualise which counties within the selected state had the most sightings.</p>

<h3>Comparative Analysis</h3>  
<p> I want to compare sightings within the selected state in 3 different ways: 
<ol>
  <li>The season in which reports were made</li>
  <li>The month in which reports were made </li>
  <li>The class types of reports made</li>
</ol>

In order to identify any patterns or trends with when these reports were made.</p>

<h3>Potential Biases</h3>



<H2>Approach</H2>

<h3>Data Collection</h3>
<p>To collect the data used for this analysis I downloaded an Excel file within the Cisco 'Introduction to Tableau module' in my Data Analytics Essentials course.</p>

<h3>Data Cleaning</h3>
<p>First I put a filter on the entire date in order to make the cleaning process easier, I then removed the 'Submitted Date' column as this was irrelevant to my analysis. Then I used conditional formatting on the year column in order to highlight any rows of data that were outside the range of 1950 - 2018. After this, I filtered all the class C reports and removed them from the dataset as they were not deemed credible enough for the analysis. I then filtered all the 'unknown' cells in the 'Season' column and removed these rows of data as they would've affected my comparative analysis later during the project, I also filtered all the '(blanks)' cells in the month column in order to remove the lines of data that didn't have a specific month as these lines of data would affect my upcoming comparative analysis.</p>

<h3>Analysis</h3>  
<p>Using a pivot table I put the state column in the row and values fields and then I sorted the data descending by 'Count of State' which showed me that Washington had the highest number of sightings (506).</p>

<p>I then created a second pivot table. This time I put 'State' and then 'County' in the Rows field and then I put 'Count of County' in the Values field in order to show sightings per county. I then sorted the data descending by 'Count of County', and then I filtered on the state of Washington in the Row field, as this was the state with the most sightings, which showed me that 'Pierce' was the county with the most sightings.</p>  



<h2>Visualisations</h2>
<a href="https://public.tableau.com/app/profile/deiniol.ampomah/viz/BigfootSightings_16995777430520/BigfootSightings1"> <img src="https://github.com/DkOwusuA004/Bigfoot-Sightings/assets/139594033/45f3179c-c7c2-4acd-a123-a800a1676d0c" alt="Bigfoot Sightings Dashboard 1">
</a>

<a href="https://public.tableau.com/app/profile/deiniol.ampomah/viz/BigfootSightings_16995777430520/BigfootSightings1"><img src="https://github.com/DkOwusuA004/Bigfoot-Sightings/assets/139594033/8266bedf-bb0d-46ef-b8dc-5a648bfc88cd" alt="Bigfoot Sightings Dashboard 2"></a>




<h2>Interpretation</h2>
<p>Within the first dashboard are 2 graphs; 'Bigfoot sightings by State' and 'Washington sightings by County'. The 'Bigfoot sightings by State' shows us that Washington produced the most Bigfoot sightings (503) between 1950-2018. This answers the first question "Which state within the USA had the most sightings over the period?".</p>

<p>In order to answer the second question; "Within this state which county was responsible for the majority of these sightings?", we have to look at the 'Washington sightings by County' graph. This graph shows us that within Washington, the county with the highest number of sightings is Pierce County with 68 sightings in the period</p>

<p>Regarding the comparative analysis we can look at tables 'Sightings by season', 'Sightings by month' and Sightings by class'.</p>

<p>Firstly, by looking at the 'Sightings by season' graph, we can see that 40.36% of sightings (203) were reported during Summer, this could be due to... . We can also see that the month with the lowest number of sightings reported was winter with 59 sightings over the period. This could be caused by...</p>

<p>Next, looking at the 'sightings by month' graph, we can see that the month of August had 88 sightings reported out of a possible 503 (11.73%). This graph shows us that the summer sightings were greatly influenced by the month of August as the 2nd and 3rd highest months after August were October (68) and September (67) </p>

<p>Finally, the 'sightings by class' graph shows that the majority (58.65%) of reports made were reports involving incidents where a possible sighting was observed at a great distance or in poor lighting conditions </p>
<h2>Potential Biases</h2>



<h2>Technologies</h2>
<img src="https://download.logo.wine/logo/Microsoft_Excel/Microsoft_Excel-Logo.wine.png" alt="Excel Logo" width="150" height="100">

<img src="https://github.com/DkOwusuA004/Bigfoot-Sightings/assets/139594033/1004ca36-cdf6-4025-8456-f38320fbb42b" alt="Tableau Public Logo" Width="150" height="80">


<h2>Setup</h2>

<h2>Status</h2>
<p><img src="https://geps.dev/progress/100" height="50" width="200"></p>


<h2>Credits</h2>
<a href="https://skillsforall.com/launch?id=1b81c11b-147b-49aa-8f87-a3469f24d280&tab=curriculum&view=db1d06b1-3987-55fa-8268-eaa0a91a802f&showContentView">Moudle 8.1 - Introducing Tableau</a>
