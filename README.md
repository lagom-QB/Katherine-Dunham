![Status](https://img.shields.io/badge/status-wip-color)
![Status](https://img.shields.io/badge/status-incomplete-color)

# Katherine Dunham

Katherine Dunham was a dancer and choreographer. This data contains information about her works from _1937 - 1962_.

With this project, I aim to gain insights  about Katherine Dunham on:

- Performances
- Impact
- Cultural influence

Generally, I want to look at her _contribution to art and the cultural landscape_

____

## Progress

### Understanding the columns  

<pre>
- Work: The common name of the piece
- Also Known As: Alternative names and variations of the piece
- Years Performed: Years between 1937 - 1962 in which the piece was performed
- Number of Events Documented: Approxiamte number of programs and printed documents referencing the performance
- Performers (only for Pieces and Mixed Works): Featured performers
- Category: Type of performance
- Named Dances in Dances: If the Category is a "Piece" or "Mixed Work"
- Pieces: If the Category is "Container", "Mixed Work" or "Show" or if the Category is "Dances in Dances"
- Mixed Works (Sometimes Piece or Container): If the Category is "Container" or "Show" or if the Category is "Dances in Dances" or "Pieces"
- Act-Length Containers: If the Category is "Show" or if the Category is "Mixed Work" or "Pieces"
- Named Evening-Length Shows: If the Category is "Works", "Container" or "Pieces"
- Program Notes (Indicative?): Represent the common notes that appeared in programs for each performance
- Place Inspiration: Preservation of Dunham's descriptive language in program notes
- Composers: Attribution
- Venue: c -> Concert hall n -> Night club
- Notes: Explanatory notes
- Sources: Source of materials
</pre>

### Cultural Influence
Cultural influence would be about the 'Program Notes', 'Place Inspiration', '??Named Dances in Dances'  

- The ___Program Notes___           : _Tells us the common story being described_
- The ___Place Inspiration___       : _Where is inspiration for this story taken from?_
- __Category__ : _What type of piece was this_
- ___Named Dances in Dances___      : _Other cultures incorporated_
- ___Years Performed___             : _How long were people interested in this story?_
- ___Number of Events Documented___ : _For how long were people interested in this story?_

The countries and regions are important as they give an idea of what is happening.  
I realised there are a lot of places listed in the _Program notes_ and the _place inspiration_.  

Now I got interested in connecting these places with _Years Performed_ and _Number of Events Documented_

<div style="border-bottom: .15rem solid grey;width: 75%; margin:0rem .2rem 0rem .4rem"></div>
<br>
<pre>
- Of the 278 works, 78 works have a country or region mentioned in the Program Notes and 77 works have a country or region in the Place Inspiration.
- The maximum number of events documented is 177 over a period of 17 years, from 1939-1962
- 4 Works were never documented:
  - Drum Session
  - Octaroon Ball
  - Spanish Earth Suite
  - Clarence
- 47 works documented once
- It's also important to know what years the Works were performed. Of the 276 works, 157 have 'Years Performed' values.
- Of the categories they are split into:
  - 111 Piece/Standalone
  - 80 Piece
  - 46 Dance
  - 22 Container
  - 9 Show
  - 8 Mix
</pre>

Because I'm trying to acertain which years were influenced by what countries, I'm eliminating the data without _Years Performed_ and the _Notes Countried_ and _Inspiration Countries_ without values which leaves me with 93 rows of the initial 276.

<div style="border-bottom: .12rem solid grey;width: 75%; float: right;"></div>
<br>
<pre>

Looking at the data currently, the _Program Notes_ column contains nan values. Not bad ...

The _Notes Countries_ also contains a lot of empty rows.  

It doesn't make sense that the _Erzulie Moundong_ has 1 Event documented but was performed in 1946 and 1947 ! _So I'm excuding it because it is just not possible_

Sooo ...  
Q1. Where does she get inspiration from?  
... This must have to do with the _Place Inspiration_ and the consequent _Inspiration Countries_
</pre>
<div style="border-bottom: .12rem solid grey;width: 75%; float: left;"></div>
<br>
<pre>

I can conclude that most of her cultural inspiration was taken from _Haiti, United States, Cuba_ and _Brazil_

Now what cultures did she influence ? 

The _Named Dances in Dances_ are not _Work_  URGHHHH   
The next thing is to look at what _Work_ has common _Named Dances in Dances_  in a density plot?
</pre>