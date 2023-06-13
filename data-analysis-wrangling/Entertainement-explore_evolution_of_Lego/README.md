# Exploring the evolution of Lego
![yulia-matvienko-kgz9vsP5JCU-unsplash](https://github.com/xaviermmi/academic-projects/assets/122324304/d02e1192-c167-4da7-aa11-f29bace03689)

## 1. Introduction
<p>Lego is a household name across the world, supported by a diverse toy line, hit movies, and a series of successful video games. In this project, we are going to explore a key development in the history of Lego: the introduction of licensed sets such as Star Wars, Super Heroes, and Harry Potter.</p>
<p>It may not be widely known, but Lego has had its share of ups and downs since its inception in the early 20th century. This includes a particularly rough period in the late 90s. As described in <a href="https://www.businessinsider.com/how-lego-made-a-huge-turnaround-2014-2?r=US&IR=T">this article</a>, Lego was only able to survive due to a successful internal brand (Bionicle) and the introduction of its first licensed series: Star Wars. In the instructions panel are the two questions you will need to answer to complete this project.</p>
<p>Before diving into our analysis though, let's become familiar with the two datasets that will help you with this project:<br></p>

<h3 id="letslookatlegosets">Let's look at Lego sets!</h3>

<div style="background-color: #ebf4f7; color: #595959; text-align:left; vertical-align: middle; padding: 15px 25px 15px 25px; line-height: 1.6;">
    <div style="font-size:20px"><b>datasets/lego_sets.csv</b></div>
<ul>
    <li><b>set_num:</b> A code that is unique to each set in the dataset. <b><i>This column is critical, and a missing value indicates the set is a duplicate or invalid!</i></b></li>
    <li><b>set_name:</b> A name for every set in the dataset (note that this can be the same for different sets).</li>
    <li><b>year:</b> The date the set was released.</li>
    <li><b>num_parts:</b> The number of parts contained in the set.<b><i> This column is not central to our analyses, so missing values are acceptable.</i></b></li>
        <li><b>theme_name:</b> The name of the sub-theme of the set.</li>
    <li><b>parent_theme:</b> The name of the parent theme the set belongs to. Matches the `name` column of the `parent_themes` csv file.</li>
</ul>

<div style="font-size:20px"><b>datasets/parent_themes.csv</b></div>
<ul>
    <li><b>id:</b> A code that is unique to every theme.</li>
    <li><b>name:</b> The name of the parent theme.</li>
    <li><b>is_licensed:</b> A Boolean column specifying whether the theme is a licensed theme.</li>
</ul>
    </div>

## 2. Project Instructions
Just like if we were a Data Analyst at Lego working with the Sales/Customer Success teams, we will try to get specific information in preparation for the meeting between the Account Executive responsible for the Star Wars partnership at Lego, and the Star Wars team. Although Star Wars was critical to the survival of the brand, Lego has since introduced a wide variety of licensed sets over subsequent years.

Here are the two questions we would like to answer:

1. **What percentage of all licensed sets ever released were Star Wars themed?** 

2. **In which year was Star Wars not the most popular licensed theme (in terms of number of sets released that year)?**

## 3. Skills
This project is showcasing <code>pandas</code> Data Manipulation skills such as :
<li>validating data types and describing basic statistics 
<li>cleaning data : na, duplicates, naming, reshaping, etc...
<li>merging dataframes
<li>running specific analysis to answer business questions as described in following instructions panel.</li>

## 4. Project summary
The project notebook is organized in 4 parts :
<li>Import library & load data
<li>Data validation
<li>Cleaning
<li>Merging
<li>Answering 1st question : proportion of licensed sets that are related to Star Wars
    <ul>>will be saved as a variable the_force in the form of an integer - e.g. 25.</ul>
<li>Answering 2nd question : which year was Star Wars NOT the most popular license ?
    <ul>>will be saved as a variable new_era in the form of an integer - e.g. 2012.</ul>
</li>
