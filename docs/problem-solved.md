---
layout: default
title: مسائل حل شده
nav_order: 5
---

# مسائل حل شده


**بزودی ...**


<!-- {: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Main navigation

The main navigation for your Just the Docs site is on the left side of the page at large screens and on the top (behind a tap) on small screens. The main navigation can be structured to accommodate a multi-level menu system (pages with children and grandchildren).

By default, all pages will appear as top level pages in the main nav unless a parent page is defined (see [Pages with Children](#pages-with-children)).

---

## Ordering pages

To specify a page order, use the `nav_order` variable in your pages' YAML front matter.

#### Example
{: .no_toc }
```yaml
---
layout: default
title: resource
nav_order: 4
---
```

---

## Excluding pages

For specific pages that you do not wish to include in the main navigation, e.g. a 404 page or a landing page. Use the `nav_exclude: true` parameter in the YAML front matter for that page.

#### Example
{: .no_toc }
```yaml
---
layout: default
title: 404
nav_exclude: true
---
```

---

## Pages with children

Sometimes you will want to create a page with many children (a section). First, it is recommended that you keep pages that are related in a directory together... For example, in these docs, we keep all of the written documentation in the `./docs` directory and each of the sections in subdirectories like `./docs/ruby` and `./docs/ror`. This gives is an organization like:

```
+-- ..
|-- (Jekyll files)
|
|-- docs
|   |-- ruby
|   |   |-- ruby.md  (parent page)
|   |   |-- buttons.md
|   |   |-- code.md
|   |   |-- labels.md
|   |   |-- tables.md
|   |   +-- typography.md
|   |
|   |-- ror
|   |   |-- ror.md      (parent page)
|   |   |-- color.md
|   |   |-- layout.md
|   |   |-- responsive-modifiers.md
|   |   +-- typography.md
|   |
|   |-- (other md files, pages with no children)
|   +-- ..
|
|-- (Jekyll files)
+-- ..
```

On the parent pages, add 2 YAML front matter variables:
-  `has_children: true` (tells us that this a parent page)
-  `permalink:` set this to the site directories that the contains the pages

#### Example
{: .no_toc }

```yaml
---
layout: default
title: ruby
nav_order: 2
has_children: true
permalink: /docs/ruby
---
```

Here we're setting up the ruby landing page that is available at `/docs/ruby`, it has children and is ordered second in the main nav.

### Child pages
{: .text-gamma }

On child pages, simply set the `parent:` YAML front matter to whatever the parent's page title is and set a nav order (this number is now scoped within the section).

#### Example
{: .no_toc }
```yaml
---
layout: default
title: Buttons
parent: ruby
nav_order: 2
---
```

The Buttons page appears a child of ruby and appears second in the ruby section.

### Children with children
{: .text-gamma }

Child pages can also have children (grand children). This is achieved by using a similar pattern on the child and grand child pages.

1. Add the `has_children` attribute to the child
1. Add the `parent` and `grand_parent` attribute to the grandchild

#### Example
{: .no_toc }

```yaml
---
layout: default
title: Buttons
parent: ruby
nav_order: 2
has_children: true
---
```

```yaml
---
layout: default
title: Buttons Child Page
parent: Buttons
grand_parent: ruby
nav_order: 1
---
```

Would create the following navigation structure:

```
+-- ..
|
|-- ruby
|   |-- ..
|   |
|   |-- Buttons
|   |   |-- Button Child Page
|   |
|   |-- ..
|
+-- ..
```

---

## Auxiliary Navigation

To add a auxiliary navigation item to your site (in the upper right on all pages), add it to the `aux_nav` [perface option]({{ site.baseurl }}{% link docs/perface.md %}#aux-nav) in your site's `_config.yml` file.

#### Example
{: .no_toc }

```yml
# Aux links for the upper right navigation
aux_links:
"Just the Docs on GitHub":
    - "//github.com/pmarsceill/just-the-docs"
```

---

## In-page navigation with Table of Contents

To generate a Table of Contents on your docs pages, you can use the `{:toc}` method from Kramdown, immediately after an `<ol>` in markdown. This will automatically generate an ordered list of anchor links to various sections of page based on headings and heading levels. There may be occasions where you're using a heading and you don't want it to show up in the TOC, to skip a particular heading use the `{: .no_toc }` CSS class.

#### Example
{: .no_toc }

```markdown
# Navigation Structure
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
```

This example skips the page name heading (`#`) from the TOC, as well as the heading for the Table of Contents itself (`##`) because it is redundant, followed by the table of contents itself. -->
