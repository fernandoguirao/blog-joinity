---
layout: post

title: Welcome to Joinity
subtitle: "What's in the box"
cover_image: blog-cover.jpg

excerpt: "Cras mattis consectetur purus sit amet fermentum. Cras mattis consectetur purus sit amet fermentum."

author:
  name: Fernando Guirao
  twitter: fguirao
  gplus: 2323123123 
  bio: Co-founder, Product design
  image: ks.png
---

Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.

Cras mattis consectetur purus sit amet fermentum:

{% highlight yaml %}
layout: post

title: Welcome to Joinity
subtitle: "What's in the box"

# Setup post cover image in /images/
cover_image: blog-cover.jpg

excerpt: "Cras mattis consectetur purus sit amet fermentum purus sit amet fermentum."

# Author details, including Google Plus authorship
author:
  name: Fernando Guirao
  twitter: fguirao
  gplus: 2392394234823 
  bio: Co-founder, Product design
  image: ks.jpg
  
# Keep it as draft, not published in index.html or feed.xml
draft: false
{% endhighlight %}

#### Configurable & Code Snipped Highlighting

/assets/stylesheets/main.scss:
{% highlight scss %}

/* Bodytext font */
$font: "Droid Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;

/* Font for headings */
$fontheadings: "Droid Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;

/* Text colors */
$text: #21272d;
$textmuted: #848484;
$accent: #2077b2;    
{% endhighlight %}

config.yml:
{% highlight yaml %}
inc:
  # Blog Information
  title:        "Joinity, the join community"
  subtitle:     "News and updates from joinity.com"
  cover_image:  blog-cover.jpg
  
  # Company information
  company:      Joinity
  url:          http://joinity.com/
  facebook:     joinity
  twitter:      joinity
  about_link:   https://joinity.com/about/
  
  # Product Information
  product_link: http://joinity.com/
  tagline:      "News and updates from joinity.com"
  
  # Comments
  disqus:
    # Eg. "exampleblog" Set to false to disable comments
    shortname:  false
  
  
  # Sharing settings
  sharing:
    twitter:    false
    facebook:   false
    gplus:      false
    hn:         false
    
  
 # Analytics     
  analytics:
    google: 
      # eg. 'UA-123-12'
      id:       false    
{% endhighlight %}

**Zoomable images**
<div class="full zoomable"><img src="/images/incorporated.jpg"></div>

**Awesome quotes**
> “Effective companies tend to communicate more, their people are curious and they have opinions”

Stay tuned for updates.