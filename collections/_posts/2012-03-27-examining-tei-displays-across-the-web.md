---
author: carin-yavorcik
date: 2012-03-27 14:00:13+00:00
layout: post
slug: examining-tei-displays-across-the-web
title: Examining TEI Displays Across the Web
categories:
- Digital Humanities
tags:
- Digital Humanities
- TEI
---

As part of my project with [Zane](http://www.scholarslab.org/author/zschwarzlose/) to update the [TEIDisplay plugin for Omeka](http://www.scholarslab.org/digital-humanities/an-update-to-teidisplay-for-omeka/), I have been examining ways that different digital collections present TEI-encoded texts. We hope that by looking at the ways that other display tools function, we’ll be able to gain more insight into what works well and what doesn’t.

One of the first sites I looked at was _[Thomas MacGreevy and George Yeats: A Friendship in Letters](http://www.macgreevy.org/collections/gyeats/index.html), _a collection of letters spanning 1922-1965. What first stands out about this collection is the two-paned display. On either side, users can choose from a set of tabs how they want to examine each letter – annotated text, scanned page images, bibliographic information from the letter’s teiHeader, and biographic information about people mentioned in the letter. This setup makes it easier to display necessary information depending on what a user’s goals are.

The display of the TEI text itself also includes some nice features. Most letters have scholarly annotations that default to displaying in superscript – readers click on the note indicator and get a pop up box displaying the note, or they can click a button to hide notes entirely and read the letter as is. The encoded texts also display some of the visual features of the original letters, such as noting deletions with a strikethrough and additions with superscript text. The effect is a nice example of how digital editions of scholarly texts can combine different editorial practices such as social or documentary editing, as the MacGreevy Archive editor, Susan Schreibman, notes in her article about the collection, “The Lives of Others: Editing Online Editions of Correspondence,” from _Digital Scholarship._

The setup of the [Victorian Women Writers Project](http://webapp1.dlib.indiana.edu/vwwp/welcome.do) at Indiana University is very different. The focus here is more specifically on the encoded text body of the materials, primarily prose and poetry written by British women of the 19th century. The display is simple but effective. A table of contents runs along the left hand side of the page, giving users a way to navigate through each document. When notes occur in the text, they are displayed at the bottom of each page as footnotes. Additionally, users can download the XML if they so choose.

Though page images are not available for most of the materials in the Women Writers Project collection, the system does have the capability to display them, as is evidenced by one of the other Indiana University collections, the [Brevier Legislative Reports](http://webapp1.dlib.indiana.edu/brevier/welcome.do), which uses the same display tool. If a user would like to examine an image of a page, she can click the “view page” link next to the page number indicator, and a pop-up image appears. However, this image does in some cases cover the encoded text, which makes it a little harder to compare the two. Alternatively, where these page images are available, a user can switch directly to “image mode” and read the page images without the encoded text, or download the whole document as a PDF.

I also explored the classics texts at the [Perseus Digital Library](http://www.perseus.tufts.edu/hopper/) at Tufts University, which offers a lot of interesting interactive features with the display of its TEI text. Like the Victorian Women Writers site, there is a table of contents on the left-hand side to facilitate navigation. Through a series of tools on the right-hand side of the page, users can choose to display different editions and/or translations of a work, including editions of scholarly annotations. Additionally, place names are automatically extracted from the TEI text and can be searched or visualized in a network or on a map. Users can also jump back and forth between commentary or cross-references to the work, and the site also offers the ability to search within a specific document or discover how words are used throughout a work.

There were two main features that really stood out to me when evaluating these projects. One was that for the longer texts, it was really helpful to have the table of contents feature that allowed for easier browsing. The original version of TEIDisplay did have an option to render documents as “segmental” with a similar table of contents – this is definitely a functionality we’d like to keep, so we’ll be experimenting with it as we update the plugin.

Another feature I really liked in exploring the projects above was flexibility. It was nice to have the opportunity to customize the view you want to what your needs are – whether it’s hiding scholarly annotations, pulling up page images, or comparing editions. We are currently working on one viewing option that is progressing well – the ability to associate page images with encoded text. Overall, though, it may harder for us to implement something really flexible on the user end out of the box, given that we are not designing for a specific collection with specific needs. Rather, we are trying to make a general tool that works in many situations, which can be easily customized on the designer end to fit different collection needs as necessary. With something so general, it’s impossible to plan for all flexibility options that users may desire. But we hope that with really robust documentation about how everything works in the plugin, the creators of digital collections may be able to get in and tinker “under the hood” to customize the display as necessary.