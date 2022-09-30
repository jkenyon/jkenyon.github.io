---
title: Off-Campus Access Tools
nav: true
---

# Off-Campus Access Tools

**What you'll find on this page:**
- <a href="#bookmarklet">UI Log-in Bookmarklet</a>
- <a href="#vpn">UI Virtual Private Network</a>

<a id="bookmarklet"></a>
{% capture text %}
<a id="source"></a>

#### Source
Created by the University of Idaho Library.  **Get the bookmarklet [here](https://www.lib.uidaho.edu/find/articles.html#tools).**

<a id="whatisit"></a>

#### What is it?

The log-in bookmarklet allows you to <a href="{{ '/content/0-Concepts.html' | relative_url }}">authenticate</a> through the UI from wherever you are on the internet without leaving that page.

<a id="value"></a>

#### Why would you use it?

About 70% of academic journal literature is estimated to be subscription-only \([Piwowar, 2018](https://peerj.com/articles/4375/)\).  For the UI community, the UI Library subscribes to a large part of this literature.  However, to gain access, the website where the article is located must recognize your affiliation with the UI.  The bookmark lets you do this with a single click, followed by your usual login method.

<a id="howitworks"></a>

#### How does it work?

When you click the bookmark, the browser is instructed to take your current url, such as  
[https://wildlife.onlinelibrary.wiley.com/doi/full/10.1002/jwmg.72](https://wildlife.onlinelibrary.wiley.com/doi/full/10.1002/jwmg.72)
and prepends the UI Library authentication url to it.  Then it reloads the page.  In order to proceed, the browser will ask you to log in.  When you do, a temporary cookie is stored on your machine that tells websites that you are affiliated with the University of Idaho.  In the case of journal articles, if we subscribe, you get access.

{% capture text %}
**Remember!** You cannot authenticate for websites that have nothing to do with academic literature.  So, if you try it using something that has nothing to do with the UI Library, such as ESPN.com, you’ll just get an error.
{% endcapture %}
{% include alert.md text=text %}

At a more general level, bookmarklets work by passing some browser-readable content into the browser’s queue.  Typically, when you create a bookmark, you just save a URL and on accessing it, you reload the page to that url (and/or create a new tab, etc.)  However, you can rewrite the bookmark content to run a javascript action instead.  In this case, we re-route the same url through the authentication system (UI Library's proxy server):
```javascript:void(location.href=%22http://ida.lib.uidaho.edu:2048/login?url=%22+location.href)```

<a id="howtouseit"></a>

#### How Do You Use it?

It's very simple!

1. Go to the UI Off-Campus Access Page
2. Drag the link to your bookmarks
3. Click whenever you want to authenticate

Alternatively, you can create a bookmark or save a favorite (depending on your browser type), and replace the url with the javascript code above.  It should work exactly the same!

<a id="privacy"></a>

#### Privacy Concerns

There are no unique privacy concerns beyond the use of cookies for authentication through the University of Idaho's Information Technology Services systems, which occurs every time one logs in to use VandalWeb, Web Mail, or any other University of Idaho service.  The UI Library collects no data from this process.

<a id="limitations"></a>

#### Limitations

1. The first limitation is obvious.  The Library must subscribe to the journal!  If not, then it won’t work.  The bookmark does not make things available that otherwise would not be. 
2. The second limitation is that it only works for items that we have registered in our system.  For…reasons…, there may be a domain or two that we subscribe to, but that we have failed to register in our authentication system.  If you receive an error, this may be the case.


{% endcapture %}
{% include card.md text=text header="UI Login Bookmarklet" %}

<a id="vpn"></a>
{% capture text %}
<a id="source"></a>

#### Source
University of Idaho Information Technology Services.  **Get the VPN tool [here](https://support.uidaho.edu/TDClient/Requests/ServiceDet?ID=599).**

<a id="whatisit"></a>

#### What is it?

A Virtual Private Network (VPN) provides a secure (encrypted) connection to the University of Idaho's network from off campus. You must have VPN access approved before you can connect to University of Idaho's network from home or while traveling.

<a id="value"></a>

#### Why would you use it?

Most journals authenticate using the University’s IP address range, meaning, they will recognize you as affiliated with the UI regardless which device you use on the campus – they will recognize your phone, tablet, laptop, desktop, etc.  When you connect using the VPN Tool, you establish a private network relationship with the UI campus network.  Then, journals treat you the same as if you are connecting at the UI campus.

<a id="howitworks"></a>

#### How does it work?

\"VPNs can be characterized as host-to-network or remote access by connecting a single computer to a network, or as site-to-site for connecting two networks. In a corporate setting, remote-access VPNs allow employees to access the company's intranet from outside the office.\" [Wikipedia, 2019](https://en.wikipedia.org/wiki/Virtual_private_network) 

<a id="howtouseit"></a>

#### How Do You Use it?


1. You first need to go to the [VPN Access](https://support.uidaho.edu/TDClient/Requests/ServiceDet?ID=599) page for ITS.  You must request access and be approved.  When that occurs, you’ll need to download the VPN client from ITS according to your operating system.

2. Once [installed](https://support.uidaho.edu/TDClient/KB/ArticleDet?ID=40), you click on ‘Connect’ and log in.  Then you’re done!

<a id="privacy"></a>

#### Privacy Concerns

The primary concern with the VPN is that you are connected to the UI while the VPN is active.  This means that everything – *everything* – you do online while connected is routed through and visible on the UI servers to ITS personnel.  If using a personal device, keep this in mind.  If you use a VPN to connect for research purposes, disconnect before moving on to personal uses.  Your private business is not for the University to see and hear and/or record – it is a public institution.

<a id="limitations"></a>

#### Limitations

The primary limitation is the need to connect and disconnect and to remember to do so.

{% endcapture %}
{% include card.md text=text header="UI Virtual Private Network" %}