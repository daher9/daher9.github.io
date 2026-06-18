---
layout: post
title: "Template"
date: 2026-06-18 11:03:00 +0200
tag: test
excerpt: "A comprehensive testing template for Jekyll and Liquid syntax structures."
published: true
---

## 1. Site and Page Variables
Jekyll uses double curly braces `{{ }}` to output variables defined in your front matter or `_config.yml` file.

* **Page Title:** {{ page.title }}
* **Post Date:** {{ page.date | date: "%B %d, %Y" }}
* **Site Name:** {{ site.title }}
* **Site Email:** {{ site.email }}

---

## 2. Filters (Data Manipulation)
Filters change the output of a variable using the pipe `|` symbol.

* **Uppercase:** {{ "hello world" | upcase }}
* **Lowercase:** {{ "HELLO WORLD" | downcase }}
* **Word Count:** This post has {{ content | number_of_words }} words.
* **Slugify text:** {{ "Jekyll Is Awesome!" | slugify }}

---

## 3. Conditionals (If/Else Logic)
Control what displays on the page based on specific conditions.

{% if page.published == true %}
🟢 This post is actively published.
{% else %}
🔴 This post is a draft.
{% endif %}

{% if site.twitter_username %}
Follow the author on Twitter: @{{ site.twitter_username }}
{% endif %}

---

## 4. Loops (Iterating Collections)
You can loop through your site's posts, pages, or custom navigation arrays.

### Recent Posts List
<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> 
      ({{ post.date | date: "%Y-%m-%d" }})
    </li>
  {% endfor %}
</ul>

---

## 5. Include Snippets
Reuse components across your site (files must live inside the `_includes/` folder).

{% include social-links.html %}

### Passing Parameters to Includes
{% include alert.html type="warning" message="This is a custom alert message!" %}

---

## 6. Internal Linking (Safe URL Paths)
Never hardcode absolute links. Use the `link` or `relative_url` tags so paths don't break on GitHub Pages.

* **Link to a file:** [Contact Page]({{ site.baseurl }}{% link contact.md %})
* **Link to an asset:** <img src="{{ '/assets/images/logo.png' | relative_url }}" alt="Logo">

---

## 7. Code Highlighting (Pygments/Rouge)
Jekyll has built-in support for code syntax highlighting using the `highlight` tag block.

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
{% endhighlight %}

---

## 8. Excerpts
You can manually define where a post preview ends on your homepage using an explicit separator tag.

This sentence will show up on the homepage index loop.
<!--more-->
This sentence will only show up when a user clicks into the full post view.
