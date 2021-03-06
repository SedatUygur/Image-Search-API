# Author
![@Rafase282](https://avatars.githubusercontent.com/u/90511329?s=128&u=8de1c9bd1ac0d19533748f20d1cf3486aa45c667&v=4)

Created by Sedat Can Uygur

[Github](https://github.com/SedatUygur) | [FreeCodeCamp](http://www.freecodecamp.com/pcengineer48) | [CodePen](http://codepen.io/SedatUygur) | [LinkedIn](https://www.linkedin.com/in/sedat-can-uygur) | [E-Mail](mailto:sedatcan_92@hotmail.com)

# Image Search API
## User stories:
1. I can get the image URLs, alt text and page urls for a set of images relating to a given search string.
2. I can paginate through the responses by adding a ?offset=2 parameter to the URL.
3. I can get a list of the most recently submitted search strings.

## Example query usage:

```text
https://img-sal.herokuapp.com/lolcats%20funny?offset=10
https://img-sal.herokuapp.com/latest
```

## Example query output:

```js
[{
  "url": "http://data.whicdn.com/images/34129178/large.jpg",
  "snippet": "this image include: funny",
  "thumbnail": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcQ9wRI3mrK8iXg7mcSZx8yfpwlR2W7dCXA3lGHvQ28SnKGsvGYt6eIflAIq",
  "context": "http://weheartit.com/entry/group/4233028"
}, {
  "url": "https://s-media-cache-ak0.pinimg.com/736x/bc/32/f3/bc32f3896ebe6cfc48d489f5e7674d7a.jpg",
  "snippet": "#lolcats funny cats:",
  "thumbnail": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQBhYqlh_TWw8ycQeSpt9MwPJLIbL7X9dFCjPpEmSyaIpMQlI-AXN75EUo",
  "context": "https://www.pinterest.com/pin/51298883228847846/"
}, {
  "url": "http://cdnstatic.visualizeus.com/thumbs/36/0b/funny,lolcat,cats,cat,lolcats,humor-360ba427d350494fb4e69b209a93a814_h.jpg",
  "snippet": "funny-pictures-cat-breaks-the-",
  "thumbnail": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcT3LYyfkNxQWcG6wmB6M2FgUZpMXbjxXhc-g4CJ18luXAvDBdBNrzXAZQ8",
  "context": "http://vi.sualize.us/funny_pictures_breaks_the_sound_barrier_lolcats_funny_cats_cat_picture_45U4.html"
}, {
  "url": "https://s-media-cache-ak0.pinimg.com/736x/41/d7/b2/41d7b23586ee2fb386d5c894abedd5ab.jpg",
  "snippet": "Saved from",
  "thumbnail": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcR8mlKrDxEzOh9PqCFiDhsdS-xwazvwTibd325l1DAUCC5dUUbq3ax9qI7M",
  "context": "https://www.pinterest.com/pin/233131718181511758/"
}, {
  "url": "http://s2.favim.com/orig/33/cat-funny-lol-lolcats-mean-Favim.com-261389.jpg",
  "snippet": "cat, funny, lol, lolcats, mean",
  "thumbnail": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTjH2_3xIIzquPGN-GVgivEQ1Ib4T9W9mCRjcYBsvLNB-e_aWb213o2-qo4",
  "context": "http://favim.com/image/261389/"
}, {
  "url": "http://cdn.playbuzz.com/cdn/d68ef92c-3973-4b00-98c9-913e423d83ff/f9ec20e0-bb55-48b1-8789-bb51947e4d12.jpg",
  "snippet": "Whats a Summary of Your life?",
  "thumbnail": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcRWWY7kdyrsQXsyW8fqoVs6_I-RwRm1BFpduC6imCrnbsbuT0Q5pmqrHrg",
  "context": "http://www.playbuzz.com/mikeyh10/whats-a-summary-of-your-life"
}, {
  "url": "http://cdnstatic.visualizeus.com/thumbs/0d/26/funny,cat,catfunny,lolcats,cute,cats-0d26770e7aaca32b2a03e601df429b17_h.jpg",
  "snippet": "funny-pictures-cat-is-excited-",
  "thumbnail": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcRDeAPTYfvumD5duVMM0OqTcyNdQeSqHM5gdm3sHSjV4w4odzQrlcSIRAI",
  "context": "http://vi.sualize.us/funny_pictures_is_excited_about_cat_funny_ribbons_lol_cats_picture_6gKf.html"
}, {
  "url": "http://cdnstatic.visualizeus.com/thumbs/ef/8f/ef8f397db7ede987b542197dcb5c2f88_h.jpg",
  "snippet": "lolcats %27n%27 funny pictures",
  "thumbnail": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcRqutfDXt3TFGEwFWpx1Wz_M8LE96eXKZssHlyPq63MVyfwCchVmi5JYwvV",
  "context": "http://vi.sualize.us/quotes_brot_youz_a_flower_lolcats_n_funny_pictures_of_cats_i_can_has_cheezbur_picture_qCWH.html"
}, {
  "url": "https://i.ytimg.com/vi/tRzXptpC3_U/hqdefault.jpg",
  "snippet": "funny lolcats and loldogs",
  "thumbnail": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcS_dKvb6pMA0bod00g0v1Bk3YakSY7H4HYwpu268AqUK8pPiSdlUh9pEnYh",
  "context": "https://www.youtube.com/watch?v=tRzXptpC3_U"
}, {
  "url": "http://data.whicdn.com/images/29044507/large.jpg",
  "snippet": "Most popular tags for this",
  "thumbnail": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcRre4NmoJmEOVxSi1VNAumtmb6nuuTpYrLlCPGuOwXXF-R34ngusPjC144",
  "context": "http://weheartit.com/entry/group/1764108"
}]
```

## Example latest output:

```js
[{
  "term": "lolcats funny",
  "when": "2016-01-23T04:21:19.441Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-23T04:20:26.237Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-23T02:06:32.898Z"
}, {
  "term": "lolcats sad",
  "when": "2016-01-23T01:29:55.894Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-23T01:29:45.727Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-23T00:43:49.365Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-22T23:47:24.660Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-22T23:43:12.142Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-22T23:35:59.976Z"
}, {
  "term": "lolcats funny",
  "when": "2016-01-22T23:13:07.220Z"
}]
```
