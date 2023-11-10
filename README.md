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
<p></p>

<h3>Data Cleaning</h3>
<p></p>

<h3>Analysis</h3>  
<p>Using a pivot table I put the state column in the row and values fields and then I sorted the data descending by 'Count of State' which showed me that Washington had the highest number of sightings (506)</p>

<p>I then created a second pivot table. This time I put 'State' and then 'County' in the Rows field and then I put 'Count of County' in the Values field in order to show sightings per county. I then sorted the data descending by 'Count of County', and then I filtered on the state of Washington in the Row field, as this was the state with the most sightings, which showed me that 'Pierce' was the county with the most sightings</p>  



<h2>Visualisations</h2>


<h2>Interpretation</h2>
<h3>Potential Biases</h3>


<h2>Technologies</h2>
Excel 
Tableau 

<h2>Setup</h2>

<h2>Status</h2>

<h2>Credits</h2>
