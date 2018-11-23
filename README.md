# html2canvas-ios-bug
微信中ios长按图片会先弹出默认浏览器菜单，然后才弹出微信中的菜单
#

![长这样](https://segmentfault.com/img/bV1SfY?w=800&h=556)
#
![长这样](https://segmentfault.com/img/bV1Sf1?w=800&h=624)

## 解决
```
  a, img {

      -webkit-touch-callout: none; /* 禁止长按链接与图片弹出菜单 */
  }
```


## 如果想完全禁止弹出菜单事件则可用
```
  img {
    point-events: none;
  }
```
