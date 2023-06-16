<h1 align="center">Awesome Brave filters</h1>
<p align="center">
A awesome list of custom content filters for Brave browser.
</p>

<p align="center">
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome" /></a>
</p>

<p align="center">
  <a href="#what-are-content-filters--">What are content filters ?</a> •
  <a href="#how-to-use">How to use</a>
  <br>
  <br>
  <a href="#filters-for-hiding-feeds">Filters for hiding feeds</a>
  <br>
  <a href="#filters-for-hiding-promoted-contents">Filters for hiding promoted contents</a>
</p>


## What are content filters ?

Content filters allows you to hide specific contents of a web-page, using a specific syntax to detect these unwanted elements.

Brave browser allows you to use predefined lists of filters, or add your own, custom filters.

This repository is a curated list of custom filters that you can use to improve your web-browsing experience.


## How to use

Go to [Brave filters settings](brave://settings/shields/filters), and copy-paste the filters of your choice in the "Create custom filters" box.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/0b9a4824-8c18-4e94-a493-d21fcc1e19d1)


## Filters for hiding feeds

<details><summary>Youtube - Welcome page</summary>

```
youtube.com##ytd-browse:has(div#header:empty)
```

Remove the videos feed displayed on the home page of Youtube.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/df4e640d-0510-45ab-8831-0d275a1f9a5a)

</details>


<details><summary>Youtube - Next videos</summary>

```
youtube.com##div#columns > div#secondary
```

When you are watching a video, remove the list of videos to watch next displayed on the right.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/ca4a75fd-74e8-493e-9926-b9187975025e)

</details>


<details><summary>StackOverflow - Hot questions</summary>

```
stackoverflow.com,stackexchange.com##div#hot-network-questions
stackoverflow.com,stackexchange.com##div#feed-link
```

Remove the list of hot questions on the right-side menu, as well as the questions feed button.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/291bad8f-75ff-4a15-8d94-1b34867f799d)

</details>


<details><summary>LinkedIn - Feed</summary>

```
linkedin.com##main > div:has(h1 + div.scaffold-finite-scroll--infinite)
```

Remove the main page's feed.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/f5bfa6d1-c78d-4d07-8c3d-4e2dbeee2fce)

</details>


<details><summary>Reddit - Feed</summary>

```
reddit.com##div[style="max-width:100%"] + div[style="max-width:100%"] > div:first-child
```

Remove the feed for any sub-reddit.

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/096ddd6f-cf63-4027-8f4d-437539a45517)

</details>


## Filters for hiding promoted contents

<details><summary>LinkedIn - Promoted posts</summary>

```
linkedin.com##div.feed-shared-update-v2:has(a[aria-label~="sponsorisé"])
linkedin.com##div.feed-shared-update-v2:has(a[aria-label~="Promoted"])
```

Remove promoted posts.

_Note : Only works if the LinkedIn interface is in French or English._

![](https://github.com/astariul/awesome-brave-filters/assets/43774355/a3df6c78-f080-47e0-8d7e-e85ebbeb3d0e)

</details>
