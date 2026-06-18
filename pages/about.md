---
title: About
layout: about
permalink: /about.html
# include CollectionBuilder info at bottom
credits: true
# featured-image value can be one objectid for a photo object in this collection, a relative path to an image in this project, or a full url to any image. If left blank, no featured image will appear at top of About page.
about-featured-image: objects/cabinet.jpg
# set background-position for featured image, "center", "top", "bottom"
position: center
# major heading to display over featured image
heading: About this Collection
# paragraph text below heading in featured image
sub-heading: 
# additional padding added to the feature to increase size. Give value in em or px, e.g. "5em".
padding: 4em
# Edit the markdown on in this file to describe your collection
# Look in _includes/feature for options to easily add features to the page
#^^ yaml frontmatter, metadata about this page
---

{% include feature/image.html objectid="frag05;frag08;frag13;frag03" width="75" %} 

## What data was used?

The data on the fragrances in this collection was manually compiled from the Parfumo/Basenotes. See below for more information about how this has been sorted.

{% capture notes %}
The [Notes](https://shidafuonline.github.io/skinscents/notes.html) page shows a visualization of the notes of the fragrances included. 

Certain notes have been tagged with a more common term to improve searchability and more accurately reflect how the prevalence is visuallized on the on this database-- for example, . 

{% endcapture %}

{% capture accords %}
The [Accords](https://shidafuonline.github.io/skinscents/accords.html) page shows all accords listed on Parfumo/Basenotes.

{% endcapture %}

{% capture location %}
The [Map](https://shidafuonline.github.io/skinscents/map.html) corresponds with places in the respective countries that the perfume houses are producing in with as much specificity as possible. As the map requires exact coordinates and perfume production is typically scattered accross laboratories, offices, and stores, the coordinates for these markers have been pulled from a business address within the country of origin listed on Parfumo/Basenotes.

{% endcapture %}

{% capture other %}

Other Data

In cases where Parfumo does not list the perfumer, this was taken from the corresponding entry on Fragrantica. 

Images of the bottles have been borrowed from the Parfumo. Any alternative text has been written independently from any that was available on the image source website. 

{% endcapture %}

{% include feature/accordion.html title1= "Notes" text1=notes title2="Accords" text2=accords title3="Location" text3=location text4=other title4="Other Data" %}



#### About CollectionBuilder CSV

This demo collection features items from the University of Idaho Library's [Digital Collections](https://www.lib.uidaho.edu/digital/), and is build using [CollectionBuilder-CSV](https://github.com/CollectionBuilder/collectionbuilder-csv).