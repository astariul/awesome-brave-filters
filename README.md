# Awesome Brave filters [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A awesome list of custom content filters for Brave browser.

* [What are content filters ?](#what-are-content-filters--)
* [How to use](#how-to-use)
* [Filters](#filters)
    + [Hiding feeds](#hiding-feeds)
        - [Youtube - Welcome page](#youtube---welcome-page)
        - [Youtube - Next videos](#youtube---next-videos)
        - [StackOverflow - Hot questions](#stackoverflow---hot-questions)
    + [Hiding promoted contents](#hiding-promoted-contents)
        - [LinkedIn - Promoted posts](#linkedin---promoted-posts)


## What are content filters ?

Content filters allows you to hide specific contents of a web-page, using a specific syntax to detect these unwanted elements.

Brave browser allows you to use predefined lists of filters, or add your own, custom filters.

This repository is a curated list of custom filters that you can use to improve your web-browsing experience.


## How to use

Go to [Brave filters settings](brave://settings/shields/filters), and copy-paste the filters of your choice in the "Create custom filters" box.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/0b9a4824-8c18-4e94-a493-d21fcc1e19d1)


## Filters

### Hiding feeds

#### Youtube - Welcome page

```
youtube.com##div#header > ytd-feed-filter-chip-bar-renderer
youtube.com##div#contents.ytd-rich-grid-renderer
```

<details><summary>Remove the videos displayed on the home page of Youtube.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/df4e640d-0510-45ab-8831-0d275a1f9a5a)

</details>

<details><summary>It also removes the feed filter at the top.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/bf7b1ba4-b48c-4147-be50-51258954eeef)

</details>


#### Youtube - Next videos

```
youtube.com##div#columns > div#secondary
```

<details><summary>When you are watching a video, remove the list of videos to watch next displayed on the right.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/ca4a75fd-74e8-493e-9926-b9187975025e)

</details>


#### StackOverflow - Hot questions

```
stackoverflow.com,stackexchange.com##div#hot-network-questions
stackoverflow.com,stackexchange.com##div#feed-link
```

<details><summary>Remove the list of hot questions on the right-side menu, as well as the questions feed button.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/291bad8f-75ff-4a15-8d94-1b34867f799d)

</details>


### Hiding promoted contents

#### LinkedIn - Promoted posts

```
linkedin.com##div.feed-shared-update-v2:has(a[aria-label~="sponsorisé"])
linkedin.com##div.feed-shared-update-v2:has(a[aria-label~="Promoted"])
```

<details><summary>Remove promoted posts.</summary>

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/a3df6c78-f080-47e0-8d7e-e85ebbeb3d0e)

</details>

_Note : Only works if the LinkedIn interface is in French or English._
