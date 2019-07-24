Short links for open science
=============================

Author: Martin Monperrus

The problem we're addressing
----------------------------

Hypertext is great in scientific papers, it enables to anchor the paper in a wide web of online references,  in order to point to posts, websites, data items, documentation pages that would not be appropriate as formal citation in the bibliography.

To add links in a paper, one has the following requirements:

* R1) the URL is short
* R2) the URL looks nice
* R3) the URL is stable over time
* R4) the scientific community has control over it

Today, many papers use off-the-shelf URL shorteners such as bit.ly or tinyurl.com. This satisfies R1, R2 and R3. The problem is that it does not comply with R4. If a malicious person takes control over the bit.ly domain name, or if a catastrophe wipes out the mapping behind tinyurl.com (or any other shortening service), it means that the scientific web of links gets broken.

The solution of l.4open.science
----------------------------

`l.4open.science` is a URL shortener by the scientific community, for the scientific community which addresses all requirements. Since we have full control over the domain name and the data, we guarantee long-term durability of the shortened URLs researchers, we guarantee that the short redirection URLs we put in papers will last for ever.

**How to add a redirection?** Create a [pull-request with a new file](https://github.com/4open-science/l/new/master) say `11.html` containing the redirection code:

```
<html><meta http-equiv="refresh" content="0; URL='https://github.com/chrislgarry/Apollo-11'"/></html>
```

In this case, this means that <http://l.4open.science/11> redirects to `https://github.com/chrislgarry/Apollo-11`.

**How to update a redirection?** Create a pull-request to update the file `11.html`, eg update [11.html](https://github.com/4open-science/l/edit/master/11.htm)

Notes
----------------------

* Universities or other academic bodies may be able to provide such a service, but I've never seen such one. I asked to several institutions without success. 
* Note that the redirection file has to end with `.html` so that <http://l.4open.science/11> is served with the proper content-type





