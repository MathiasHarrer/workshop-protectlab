---
# Title, summary, and page position.
linktitle: Chapter 1
summary: Learn how to use Wowchemy's docs layout for publishing online courses, software documentation, and tutorials.
weight: 1
icon: book
icon_pack: fas

# Page metadata.
title: Chapter 1
date: "2018-09-09T00:00:00Z"
type: book  # Do not modify.
---

<style>
code{
  color: #2a7792;
}
.hljs{
  font-size: 16px
}

</style>

## Flexibility

Document everything!

This feature can be used for publishing content such as:

* **Online courses**
* **Project or software documentation**
* **Tutorials**
* **Notes**

The `courses` folder may be renamed. For example, we can rename it to `docs` for software/project documentation or `tutorials` for creating an online course.

## Delete courses

**To remove these pages, delete the `courses` folder and see below to delete the associated menu link.**

## Update site menu

After renaming or deleting the `courses` folder, you may wish to update any `[[main]]` menu links to it by editing your menu configuration at `config/_default/menus.toml`.

For example, if you delete this folder, you can remove the following from your menu configuration:

```toml
[[main]]
  name = "Courses"
  url = "courses/"
  weight = 50
```

Or, if you are creating a software documentation site, you can rename the `courses` folder to `docs` and update the associated *Courses* menu configuration to:

```toml
[[main]]
  name = "Docs"
  url = "docs/"
  weight = 50
```

```R
library(dplyr)
a <- b
```

```python
import numpy as np
main(.)
library("dplyr")
a <- b
```

{{< highlight r >}}
library(dplyr)
a <- b
{{< / highlight >}}


```js
func
library("dplyr")
df %>%
  mutate(date = lubridate::ymd(date_string)) %>%
  select(- date_string)
str(df)
nrow(df)
```




## Update the docs menu

If you use the *docs* layout, note that the name of the menu in the front matter should be in the form `[menu.X]` where `X` is the folder name. Hence, if you rename the `courses/example/` folder, you should also rename the menu definitions in the front matter of files within `courses/example/` from `[menu.example]` to `[menu.<NewFolderName>]`.

[link](google.de)


{{< highlight R >}}
data %>%
  select(id, m, group, pss.0,
         pss.1, pss.2) %>%
  pivot_longer(-c(id, group, m),
               names_to = "time",
               names_prefix = "pss.",
               values_to = "pss") -> plot.data

jitter1 = runif(nrow(plot.data), -.05, .05)
jitter2 = runif(nrow(plot.data), -.5, .5)

within(plot.data, {
  time = as.numeric(time)
  group = as.factor(group)
  time.jitter = time + jitter1
  pss.jitter = pss + jitter2
}) -> plot.data
{{< / highlight >}}
