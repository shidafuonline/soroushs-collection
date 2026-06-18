---
title: About
layout: about
permalink: /about.html
# include CollectionBuilder info at bottom
credits: true
# featured-image value can be one objectid for a photo object in this collection, a relative path to an image in this project, or a full url to any image. If left blank, no featured image will appear at top of About page.
about-featured-image: objects/skinscentmeanswhat.png
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

{% include feature/image.html objectid="skin09;skin03;skin04;skin19;skin17" width="75" %} 

## What are skin scents?

Like much of the terminology used to describe fragrance, there is no formal definition of what constitutes 'skin scent'. Also described as "your-skin-but-better" or "perfumes for people who don't want to smell like they're wearing perfume," skin scents are typically characterized by a closer sillage (the distance from which you can smell the fragrance, also called projection), a lack of strongly discernible notes, and fragrance profiles that are generally regarded as being comforting, clean, and light.

Given their intentionally ambiguous nature, collection was built to explore the olfactory information about skin scents on the manufacturers' website that has been consolidated on the fragrance databases Fragrantica and Parfumo

## What data was used?

The data in this collection was manually compiled from the fragrance house's website (and occasionally official social media page), Parfumo/Basenotes, and Fragrantica. See below for more information about how this has been sorted.

{% capture notes %}
The [Notes](https://shidafuonline.github.io/skinscents/notes.html) page shows a visualization of the standardized notes of the fragrances included. 

Certain notes used by the perfume house have been tagged with a more common term to improve searchability and more accurately reflect how the prevalence is visuallized on the on this database-- for example, . 

{% endcapture %}

{% capture accords %}
The [Accords](https://shidafuonline.github.io/skinscents/accords.html) page shows accords from both Parfumo/Basenotes and Fragrantia. All Parfumo/Basenotes accords were included, however only the top five Fragrantica accords were included as their database can include 10+ accords per fragrance. As these have not been standardized (unlike the notes), there may be duplicates or similar notes when these databases use variations of the same word (such as Parfumo using the accord "animal" and Fragrantica using the accord "animalic"). 

{% endcapture %}

{% capture location %}
The [Map](https://shidafuonline.github.io/skinscents/map.html) corresponds with places in the respective countries that the perfume houses are producing in with as much specificity as possible. As the map requires exact coordinates and perfume production is typically scattered accross laboratories, offices, and stores, the coordinates for these markers have been pulled from a business address, stockist, or within the city or neighbourhood limits mentioned on the fragrance house's website within the country of origin listed on Parfumo/Basenotes or Fragrantica.

{% endcapture %}

{% capture other %}

Other Data

The name of the fragrance is listed as the one used by the fragrance house on their website when discrepancies between the three sources emerged, with additional information added for clarity when relevant (such as in the case of Clean, which has a scent named "Skin" in both its 'Classic' and 'Reserve' lines). 

When multiple release years were noted on the databases without the fragrance house offering this information directly, the latter year was used.

Images of the bottles have been borrowed from the fragrance house’s website whenever possible, with an alternative from Parfumo or Fragrantica being used when no stable image link was available. Any alternative text has been written independently from any that was available on the image source website. 

Perfumer names have been taken from any of the three sources, and no discrepancies emerged at the time of data collection.

{% endcapture %}

{% include feature/accordion.html title1="Notes" text1=notes title2="Accords" text2=accords title3="Location" text3=location text4=other title4="Other Data" %}



#### About CollectionBuilder CSV

This demo collection features items from the University of Idaho Library's [Digital Collections](https://www.lib.uidaho.edu/digital/), and is build using [CollectionBuilder-CSV](https://github.com/CollectionBuilder/collectionbuilder-csv).