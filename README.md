# hackernews-post-datasets

Datasets for 239,621 hackernews posts

# Descirpiton

HackerNews provides [API via Firebase](https://github.com/HackerNews/API). That lets you find all items via id that is incrementally or decremenatally. Each item represents story or comment. Since all items are represented horizontally, it is time consuming to find information you need.

This repository is the collection of top level thread (story type). That includes link share, post, SHOW HN, and ASK HN. The datasets can be used as a starting point to create hierarchical representation throuhg tracing *kids* field of each item. To focus on the popular threads only, the ones with at least 2 comments were chosen. These presets lend itself to about 1.5% of the total items.

This 239,621 datasets range from August 3, 2015 to Nov 16, 2020.

# Field

There is no alteration to the item from that returend from the original Hackernews API. Ex)

```
{
  "by" : "pc",
  "descendants" : 0,
  "id" : 100,
  "kids" : [ 454529, 152 ],
  "score" : 6,
  "time" : 1171910288,
  "title" : "SpikeSource, CA-based startup, becomes Ubuntu commercial support provider for US",
  "type" : "story",
  "url" : "http://www.linux-watch.com/news/NS7616991195.html"
}
```
