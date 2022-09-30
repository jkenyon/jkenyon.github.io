---
title: Browser Extensions
nav: true
---

# Browser Extensions

In this section, we'll describe various tools for improving ease of access and finding openly available content on the web.

**What you'll find on this page:**
- <a href="#unpaywall">Unpaywall</a>
- <a href="#oabutton">The OA Button</a>
- <a href="#lazyscholar">Lazy Scholar</a>
- <a href="#kopernio">Kopernio</a>
- <a href="#googlescholar">Google Scholar Button</a>

<a id="unpaywall"></a>

{% capture text %}

<a id="source"></a>

#### Creators
[Our Research](https://ourresearch.org), a 501(c)3 nonprofit organization based in Vancouver, B.C.  They have a number of related projects in the open science (def) domain, including Unpaywall, GetTheResearch, and Impactstory Profiles.
**Get the browser extension [here](https://unpaywall.org/products/extension).**

<a id="whatisit"></a>

#### What is it?

Unpaywall is an index and database of nearly 25 million free scholarly articles.  The database maintains descriptions of the accessibility of the journal, of the article, of the nature of access [link to types], and more.  They crawl tens of thousands of hosting locations, including institutional and disciplinary repositories, academic journal websites, and more.

<a id="value"></a>

#### Why would you use it?

Approximately 25-30% of the academic literature is open access \([Piwowar, 2018](https://peerj.com/articles/4375/)\).  This means that at least of quarter of all scholarship likely doesn't require a subscription.  However, publishers do not always link to available open versions, or the information about those versions do not travel through the various indices, catalogs, and so on.  In those cases, the Unpaywall extension will give you an indicator of whether or not there is an alternate copy available.

<a id="howitworks"></a>

#### How does it work?

The browser extension is built in Javascript \([see the code here](https://github.com/Impactstory/unpaywall)\). It scrapes the entirety of each page you visit while active, and looks for a pattern that looks like a DOI or DOI link {def}. When it finds something DOI like, it sends that to Unpaywall’s [API](https://unpaywall.org/products/api) to find the article and retrieve the relevant information. Once it obtains that, it will display the relevant icon that indicates whether or not there is a copy and the color of the type of access available.

In other words, you browse around as you would, and if you are on a page with a DOI, the extension will light up (or not) depending on whether or not you can get a copy of an article.

Try it on this article: ```https://www.nature.com/articles/s41893-019-0220-7```

<a id="howtouseit"></a>

#### How Do You Use it?

*Installation:*<br>
1. First, install the extension.  Once there, it lives in your browser and works behind the scenes.

*Use:*<br>
2. You click on the icon when you see it indicating that there is an available copy.  Otherwise, you don’t.  Easy!

*Settings:*<br>
3. There are a few settings available, but for the most part, it's a simple app.

<a id="privacy"></a>

#### Privacy Concerns

According to Unpaywall, they do not collect any personally identifiable information (PII) (def) when you use the browser extension. The extension also does not use beacons, cookies, or similar technologies. However, when you use their other services, there may be other transmissions of PII. They do collect some non-personal information – IP addresses, anonymous usage data, referring pages/URLs, browser, language used, date/time of requests made.  You may or may not agree that this is not PII; there is some disagreement about whether or not IP addresses are personal or non-personal information.
View their privacy policy [here](https://unpaywall.org/legal/privacy).

<a id="limitations"></a>

#### Limitations

The extension only works for open access content and if a DOI is listed on the page you are viewing.  If there is no open version, there will not be a link available.  It is also limited by what Unpaywall has indexed.  There may be open content that they have yet to discover and index, or that they missed.  At 25 million items, that’s probably not a common problem, but it is possible.

{% endcapture %}
{% include card.md text=text header="Unpaywall" %}

<a id="oabutton"></a>

{% capture text %}

<a id="source"></a>

#### Source
Launched 2013.  Various non-profits have funded it, included SPARC, JISC, Open Society Foundations, the Center for Open Science, and currently [Arcadia](https://blog.openaccessbutton.org/arcadia-fund-supports-open-access-button-to-improve-access-to-research-without-subscriptions-b7c36b3e1a6e). **Get the extension [here](https://openaccessbutton.org/)**.

<a id="whatisit"></a>

#### What is it?

The service, much like Unpaywall, leverages existing indices of open content and if there is an open version will provide you a link to it. In fact, it actually uses Unpaywall and others to find those open resources.

<a id="value"></a>

#### Why would you use it?

Again, approximately 25-30% of the academic literature is open access \([Piwowar, 2018](https://peerj.com/articles/4375/)\)  This means that at least of quarter of all scholarship shouldn’t require a subscription.  However, the publishers of the canonical version of the article do not always link to legally available open versions, or the information about those versions do not travel through the various indices, catalogs, and so on.  In those cases, the OA Button extension will tell you whether or not there is an alternate copy available.

The OA Button adds a unique feature though.  If the article is not found in its system, it will mediate the process of requesting an open copy from the author.  As [they say](https://blog.openaccessbutton.org/making-more-research-open-access-one-paper-at-a-time-25b95cd36c8f), major publishers permit the author to post a copy of the article in institutional repositories.  FOr most authors, it's not usually a priority and it often doesn't happen.

<a id="howitworks"></a>

#### How does it work?

The OA Button maintains a similar database and system to Unpaywall.  At one level, it works the same way, doing a automatic look-up for an article.  On another level though, they will also look up other types of identifiers and even do a fuzzy matching search for citations.  Third, they manage a request system to try and create open version of published content on a demand basis. So - unlike Unpaywall, there is a small cadre of people that help manage the request system, correspond with authors, and generally try to make more material openly available.  The benefit of this is that they are tracking the legalities therein, so you don't have to!

Try it on this article: ```https://www.nature.com/articles/s41893-019-0220-7```

<a id="howtouseit"></a>

#### How Do You Use it?

1. Install the extension.
2. When you are on a webpage with an article you need access to, or if you have a URL, DOI, PMID or PMCID and just want to find out if there is an open copy, you click on the button.  It then tells you if there is a copy, or gives you the option to create a request.
3. You can click on it to access their database and search for a DOI, Pumbed Identifier, and other identifiers.  You can also paste in a citation, but they correctly describe that as tricky; there’s a chance it won’t work.

<a id="privacy"></a>

#### Privacy Concerns

Generally, the OA Button yields the same concerns as Unpaywall. They collect information to track usage and general behavior, and with the requests system, you will be transmitting personal information, such as email addresses and your name.  (Unless you go by a pseudonym...)

View their privacy policy [here](https://openaccessbutton.org/privacy).

<a id="limitations"></a>

#### Limitations

The extension primarily works for open access content.  If there is no open version, it won't deliver a result.  It is also limited by what the OA Button and its sources have indexed.  There may be open content that they have yet to discover and index, or that they missed.  It is also possible that in the case of requests, the authors simply don't make their content open or ignore the requests.

{% endcapture %}
{% include card.md text=text header="The OA Button" %}

<a id="lazyscholar"></a>

{% capture text %}

<a id="source"></a>

#### Source
Created by [Colby Vorland](https://twitter.com/nutsci), recently a post-doctoral researcher with the Indiana University School of Public Health.  **Get the extension [here](http://www.lazyscholar.org/)**.

<a id="whatisit"></a>

#### What is it?

Unlike some of the others, this extension is focused on easing access to content using existing indices, regardless of their openness.  In fact, it has settings to enable authentication through a proxy server and quickly affiliate with UI.  It also does a number of other things, such as collect citation information, scan articles for references and other content, and export papers to reference manager software.

<a id="value"></a>

#### Why would you use it?

The author stated his intention as avoiding the "copy a title, paste into Google, copy a title, paste into Google" pattern of searching for information.  So, he leveraged his technical skill to develop an extension that gets around some of this.  If you find an item in pubmed (his field is nutrition), then Lazy Scholar will give you a relatively easy link to a copy of it...in most cases.  Using Lazy Scholar is essentially about efficiency.  If it's configured in a way that supports your research behavior, then it can save you some time and clicks.

<a id="howitworks"></a>

#### How does it work?

You have the option of setting Lazy Scholar to be active all the time, or only during your use of "scholarly" websites.  Unfortunately, there is not a clear statement of what those are, but generally, you can activiate it at any time by clicking on the Lazy Scholar button. It analyzes the page and does several things: 1) it extracts a series of useful elements for easier retrieval: outlines, supplementary materials, references, 2) it looks up the article in pubmed and retrieves some basic metrics, 3) it aims to provide links to copies of the article using a few open systems, and 4) it provides assistance with citing and with exporting a reference to a citation manager (theoretically making the citation manager extensions redundant).

Try it on this article: ```https://www.nature.com/articles/nature11723```

<a id="howtouseit"></a>

#### How Do You Use it?

1. First, install the extension.  Once there, it lives in your browser and works behind the scenes. Note - you can set it so that it only works when you click on the extension.
2. You click on the icon when you want to use it, unless you have it actively scanning everything.  In that case, it will pop up on its own.
3. The gear widget on the right takes you to the settings pages, where you can configure much of its permissions and functions.

<a id="privacy"></a>

#### Privacy Concerns

This is an interesting case.  To take the author at face value, there is little to be concerned with.  The privacy policy indicates a minimum of information collection and there seems to be a lack of interest in tracking more than that.  However, there is also a feature that requests your login credentials (for the UI) and saves it on your local system.  This creates some security concerns, so you might want to consider whether the 'efficiency' is worth that.  It might be, it's up to you.

View the 'Private Policy' [here](http://www.lazyscholar.org/private-policy/).

<a id="limitations"></a>

#### Limitations

The extension doesn't work well when there is no open copy and/or the library does not subscribe to the journal.  It is also limited in some ways by the value of the underlying tools it uses, such as Google Scholar. For example, an article on ResearchGate that is accessible through Google Scholar will be found by Lazy Scholar.  However, if that article is taken down (due to the legal issues REsearchGate currently is facing), then that can impact the value of Lazy Scholar's retrieval.  Also, if you don't use the institutional login tool, that can also limit the extension's utility.

{% endcapture %}
{% include card.md text=text header="Lazy Scholar" %}

<a id="kopernio"></a>

{% capture text %}

<a id="source"></a>

#### Source
Kopernio was acquired by Clarivate Analytics in 2018.  Clarivate is the data analytics company that operates the Web of Science, Endnote, and Journal Citation Reports, among other tools.  **Get the extension [here](https://kopernio.com/)**.

<a id="whatisit"></a>

#### What is it?

Kopernio is a freely available resource from a private company that own the Web of Science products, as well as Endnote.  Kopernio is another browser extensions that uses a series of databases to find a copy of the article that’s available on the web.  Kopernio also has a freemium model of PDF storage and sharing with others.

<a id="value"></a>

#### Why would you use it?

Kopernio's primary value is in ease of accessing materials to which you can find a copy, as well as the power of the Web of Science resource to enable quick, efficient searching.  The storage mechanism is a useful means to having a cloud-hosted storage of documents that you are using.

<a id="howtouseit"></a>

#### How Do You Use it?

1. Install the extension.
2. When you are on a webpage with an article you need access to, click on the button in the left-hand bottom corner of the screen.  It will let you know if there are any PDFs available.  If you want to search Web of Science or Pubmed, you can click on the top-right button (the extension itself), and you will be able to do a simple keyword search which will route you into your chosen database.
3. If you go to your 'locker', you can tag PDFs, search through your library, and change settings.  You can also copy a citation in dozens of styles for easy copy/pasting.

Try it on this article: ```https://www.nature.com/articles/nature11723```

<a id="privacy"></a>

#### Privacy Concerns

More so than the others on this list, Kopernio’s data collection methods need to be considered.  They do collect some personal data and use trackers to understand user behavior. The system requires that you create an account, log in, and do things within their secure environment.  Therefore, there is more tracking going on than with the other extensions on this list.  Lastly, given that Clarivate is a data analytics company, this data collection might be viewed with more suspicion than cases like Unpaywall or the OA Button (both of which are managed by non-profits focused on enabling access).  See [Kopernio’s data policy](https://kopernio.com/terms) for more details.

<a id="limitations"></a>

#### Limitations

The main limitation is that you need to create an account to really take advantage of this tool.  If you do, then you will find that you have 100MB storage for documents in the locker, and the search engine only searches Web of Science and Pubmed, so your interests may vary depending on the utility of those two systems for you.  Also, its ability to provide links to PDFs require either being on campus, or an existing open copy available.

{% endcapture %}
{% include card.md text=text header="Kopernio" %}

<a id="googlescholar"></a>

{% capture text %}

<a id="source"></a>

#### Source
Created around 2017 by Google.  **Get the extension [here](https://chrome.google.com/webstore/detail/google-scholar-button/ldipcbpaocekfooobnbcddclnhejkcpn?hl=en)**.

<a id="whatisit"></a>

#### What is it?

The Google Scholar Button treats each page like an article and looks it up in Google Scholar (which works really well for actual articles).  It then provides a shortcut to some of Google Scholar's features, like citing articles or other versions, as well as the search engine itself.

<a id="value"></a>

#### Why would you use it?

Given that Google Scholar may index upwards of 150 million items from the web, its index is possibly the largest available resource for academic literature.  The particular value of the Google Scholar Button is that you can highlight some chunk of text on a webpage and with a click of the button, you can search for items with that phrasing. It's an efficient means to finding other articles on related topics reasonably quickly.  And since it provides a proxy link for items that the UI subscribes to, it works as an alternative tool for accessing subscribed content, not just open content.

<a id="howtouseit"></a>

#### How Do You Use it?

1. First, install the extension.  Once there, it lives in your browser and works whenever you click on it.
2. You click on the icon to check Google Scholar or to search.  Otherwise, you don’t.  Easy!
3. The only settings to adjust are your Google Scholar settings.

Try it on this article: ```https://wildlife.onlinelibrary.wiley.com/doi/full/10.1002/jwmg.72```

<a id="privacy"></a>

#### Privacy Concerns

This is a Google product and carries the same concerns you might have regarding any Google product.  Keep in mind, if you are using Chrome as your browser - that's a Google product too.  

<a id="limitations"></a>

#### Limitations

This is primarily a tool that works on the back of Google Scholar, so the limitations of that index apply.  GS is rife with errors, false positives, inflated citation counts, and an inability to always identify versioning between different copies of the same thing.  It's often a remarkably valuable tool, but keep these errors in mind; it's not perfect.

{% endcapture %}
{% include card.md text=text header="Google Scholar Button" %}