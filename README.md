# Awesome Brave filters [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A awesome list of custom content filters for Brave browser.

* [What are content filters ?](#what-are-content-filters--)
* [How to use](#how-to-use)
* [Filters](#filters)
    + [Hiding feeds](#hiding-feeds)
        - [Youtube - Welcome page](#youtube---welcome-page)
        - [Youtube - Next videos](#youtube---next-videos)
        - [StackOverflow - Hot questions](#stackoverflow---hot-questions)


## What are content filters ?

Content filters allows you to hide specific contents of a web-page, using a specific syntax to detect these unwanted elements.

Brave browser allows you to use predefined lists of filters, or add your own, custom filters.

This repository is a curated list of custom filters that you can use to improve your web-browsing experience.


## How to use

Go to [Brave filters settings](brave://settings/shields/filters), and copy-paste the filters of your choice in the "Create custom filters" box.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/dc6369a2-6dfa-4329-8611-8d34783878a2)


## Filters

### Hiding feeds

#### Youtube - Welcome page

```
youtube.com##div#header > ytd-feed-filter-chip-bar-renderer
youtube.com##div#contents > ytd-rich-grid-row
youtube.com##div#contents > ytd-rich-section-renderer
```

<details><summary>Remove the videos displayed on the home page of Youtube.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/5a3e796e-4bdf-4dd2-95f9-9bd668315504)

</details>

<details><summary>It also removes the feed filter at the top.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/9318da1e-5dd8-41d2-a55c-540bede06537)

</details>


#### Youtube - Next videos

```
youtube.com##div#columns > div#secondary
```

<details><summary>When you are watching a video, remove the list of videos to watch next displayed on the right.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/2ad4b941-eb75-4f17-bd37-276dbd127644)

</details>


#### StackOverflow - Hot questions

```
stackoverflow.com,stackexchange.com##div#hot-network-questions
stackoverflow.com,stackexchange.com##div#feed-link
```

<details><summary>Remove the list of hot questions on the right-side menu, as well as the questions feed button.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/7cd17ce1-85e2-4b07-b927-9d47ffe93e73)

</details>
