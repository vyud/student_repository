---
layout: default
permalink: /pages/markdown-help/
title: Markdown Help
mathjax: true
---

## Markdown Help

You are probably curious about the text between the dotted lines visible in source view but not in your browser. This material is known as YAML frontmatter and it tells  GitHub how to process your document as part of a Jekyll website. The two triple dotted lines ('---') are the minimal items needed to indicate YAML instructions. It is used when generating this static website. If you want to add your own posts and pages to this website, use existing YAML as a guide.

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](../another-page) on this site. Look at the directory structure in your _site folder. "/another-page/" is at the same level as this page. The ".." is a shortcut that means, "go up one directory level". You can link multiple together as in '../../' to mean two levels higher. A link is further composed by adding "/" plus a directory or file.

You can also simply refer to the location of a page by it's absolute location. A shortcut on your site is to use '{{ site.baseurl }}' (which expands to {{ site.baseurl }}) and then walk out the url to the location of your file. As an example, see how the squirrel image is linked below.

Look at the formatting below and compare to the markdown from the [source file linked here]({{github_repository_url}}/edit/master/_pages/markdown-help.md) in your repository.

There should be whitespace between paragraphs.

There should be whitespace between paragraphs.

# [](#header-1)Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## [](#header-2)Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### [](#header-3)Header 3

### Inline attributes

You can embed HTML directly in markdown. It's even possible to add inline CSS. This is *red*{: style="color: red"}.

### emoji

 :smile:

### Escape Markdown
Let's rename \*this-page\* to \*that-page\*.

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### [](#header-4)Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### [](#header-5)Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### [](#header-6)Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

### Footnotes
This is some text.[^1]. Other text.[^footnote].

[^1]: Some *crazy* footnote definition.

[^footnote]:
    > Blockquotes can be in a footnote.

        as well as code blocks

    or, naturally, simple paragraphs.

### Small image from URL

![](https://assets-cdn.github.com/images/icons/emoji/octocat.png)

### Small image from repository

![]({{site.baseurl}}/assets/img/squirrel.jpg)

Note the use of '{{site.baseurl}}' which reference the base url of this site and then followed by 'assets/img/' directories and image file.

### Large image

![](https://guides.github.com/activities/hello-world/branching.png)

### Link to a downloadable presentation from repository

[My presentation]({{site.baseurl}}/public/blank_presentation.pptx)

This document is in '{{site.baseurl}}/public/'.

### Embed YouTube video (plain old HTML)

<iframe width="560" height="315" src="https://www.youtube.com/embed/mpjEyBKSfJQ?ecver=1" frameborder="0" allowfullscreen></iframe>

### Math

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

### Markdown on GitHub

There are a few things you can do with Markdown on GitHub to make working in GitHub easier. <https://help.github.com/articles/about-writing-and-formatting-on-github/>

### Esoterics

If you got this far and you are interested in see how far you can go with markdown, take a look at <https://kramdown.gettalong.org/quickref.html>.
