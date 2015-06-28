---
layout: post
title: "Author Override"
author: billy_rick
modified:
excerpt: "A post to test author overrides using a data file."
tags: []
---

For those of you who may have content written by multiple authors on your site you can now assign different authors to each post if desired.

Previously the theme used a global author for the entire site and those attributes would be used in all bylines, social networking links, Twitter Card attribution, and Google Authorship. These `owner` variables were defined in `config.yml`

Start by modifying or creating a new `authors.yml` file in the `_data` folder and add your authors using the following format.

{% highlight yaml %}
# Authors

manoj_rao:
  name: Manoj Rao
  web: http://manojrajarao.com
  email: manoj@manorajarao.com
  bio: "Your Average Common Man"
  avatar: bio-photo-2.jpg
  twitter: manojrajarao
  google:
    plus: Manoj Raja Rao

{% endhighlight %}

To assign Manoj Rao as an author for our post. You'd add the following YAML front matter to a post:

{% highlight yaml %}
author: manoj_rao
{% endhighlight %}
