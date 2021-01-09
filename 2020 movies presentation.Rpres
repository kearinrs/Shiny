2020 movies presentation
========================================================


author: Roisin Kearins

date: 09 Jan 2021

A presentation in relation to creating a Shiny app

Introduction
========================================================
This presentation is being created as part of the peer assessment for the coursera developing data products class. The assignment is to make sure that the students what they have learn and show how to apply it.

It have two part:

 - *_shiny_* to build data product application
 - *R-Presentation or slidify* to create data product related presentations
 
This project used data from IMDB based on the top 100 best movies of 2020.
(This list was accurate to the time it was updated in 2020)


The code was obtained here: https://www.imdb.com/list/ls096445020/?sort=list_order,asc&st_dt=&mode=simple&page=1&ref_=ttls_vw_smp

The 


Example of code used 
========================================================


An example of the code used was as follows:


```
dataset <- read.csv('2020_movies.csv')

fluidPage(
  titlePanel("2020_movies"),
  
  sidebarPanel(
    
    sliderInput('sampleSize', 'Sample Size', min=1, max=nrow(dataset),
                value=min(1000, nrow(dataset)), step=500, round=0),
                selectInput('x', 'X', names(dataset)),
    selectInput('y', 'Y', names(dataset), names(dataset)[[2]]),
    selectInput('color', 'Color', c('None', names(dataset))),
    
    checkboxInput('jitter', 'Jitter'),
    checkboxInput('smooth', 'Smooth'),
    
    selectInput('facet_row', 'Facet Row', c(None='.', names(dataset))),
    selectInput('facet_col', 'Facet Column', c(None='.', names(dataset)))
```
    
- The data was uploaded and a range of data selected.

What can be done in the app
========================================================


- The data can be organised by the X and Y columsn to have any of the column headers as the data marker to organise the data by any way that is more desirable.
- the sample size can easily be altered if the data source alters
- the colour scheme could be altered to be mroe astheticaly pleasing

notes for future reference:
- Could an interactive format on the plot be useful? And if so, what would the best way be?
Food for thought...

Links 
=======================================================


The application can be found on:https://github.com/kearinrs/Shiny

The source code can be found on:https://github.com/kearinrs/Shiny

The presentation can be found on: https://rpubs.com/kearinsr/711528
