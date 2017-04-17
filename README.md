## HLTV API

[![Build Status](https://travis-ci.org/dajk/hltv-api.svg?branch=master)](https://travis-ci.org/dajk/hltv-api)
[![npm](https://img.shields.io/npm/v/hltv-api.svg?maxAge=2592000)](http://npm.im/hltv-api)
[![Codecov](https://img.shields.io/codecov/c/github/dajk/hltv-api.svg?maxAge=2592000)](https://codecov.io/gh/dajk/hltv-api)
[![dependencies Status](https://david-dm.org/dajk/hltv-api/status.svg)](https://david-dm.org/dajk/hltv-api)
[![devDependencies Status](https://david-dm.org/dajk/hltv-api/dev-status.svg)](https://david-dm.org/dajk/hltv-api?type=dev)


This is small module for node.js. It's created for easier implementation data from available RSS links from [hltv.org](http://www.hltv.org/)

### Installation

```bash
$ npm install hltv-api
```

### Methods

`getLatestNews`, `getLatestBlogs`, `getLatestDemos`

##### Breaking methods (HLTV doesn't support these two anymore): `getUpcomingMatches`, `getHotMatches`

#### Get upcoming matches example
```js
import { getLatestNews, getLatestBlogs, getLatestDemos } from 'hltv-api';

getLatestNews.get((news) => console.dir(news));
getLatestNews.get((blogs) => console.dir(blogs));
getLatestNews.get((demos) => console.dir(demos));
```
