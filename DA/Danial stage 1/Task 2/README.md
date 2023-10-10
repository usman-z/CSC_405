# Task 2 Report

**Description of the enrichment data and datatype.**

* state(String) - The state of the county.
* county(String) - The county where voting occurred.
* current_votes(Integer) - The number of votes said candidate has right now for said county
* total_votes(Integer) - The number of votes said candidate received for said county
* percent(Integer) - The percent of votes said candidate received from the total votes

**How can you merge the data with the primary COVID-19 dataset? Identify the individual variable which map between the datasets.**

The essential variable that links the two datasets together is the `county` column in the secondary dataset and the `county` column in the primary COVID-19 dataset. These columns likely contain county names or identifiers that are shared between the datasets. By specifying these columns as the keys for our merge operation, we consolidate the data based on a common geographical reference.

**Describe how your enrichment data can help in the analysis of COVID-19 spread. Post initial hypothesis questions.**

This enrichment data can help in the analysis of COVID-19 spread by knowing the political orientation of a county's population can help public health officials tailor their messaging and outreach efforts effectively. Different political groups may respond differently to health recommendations and mandates. Understanding these differences can aid in crafting communication strategies that resonate with specific communities. 

*Hypothesis: Counties with more liberal values will have a lowwer COVID-19 spread.*
