# [Fusebox module import issue](https://github.com/fuse-box/fuse-box/issues/541)

![fuse-box-xstream-issue](https://cloud.githubusercontent.com/assets/736697/26168009/17d4e65c-3b52-11e7-8406-9c567a1fbebb.gif)

1) `yarn`
2) `yarn watch`
3) load `http://localhost:3000/`
4) Goto `client/app.ts` and uncomment 2 lines with `debounce`
5) Save file, page should reload, probably no error
4) Uncomment next 2 lines with `throttle`
5) Save file, page should reload, should probably see the error:
```
TypeError: Cannot read property 'default' of undefined
```
