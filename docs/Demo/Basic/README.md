---
sidebarDepth: 2
---

# Basic Demo

## 1.Basic scroll

#### Vuescroll and native both support basic scroll behaviors. But vuescroll scrolls more smoothly and have a pretty surface.

<ClientOnly>
<Demo-Basic-OrdinaryScroll />
</ClientOnly>

## 2.Customize position

#### Vuescroll supports setting the positions of the scrollbar and rail or keep show while native doesn't.

<ClientOnly>
<Demo-Basic-SetPositionAndKeepShow />
</ClientOnly>

## 3.Detect size changes

#### Vuescroll supports detecting the size changes of content and native doesn't. It is inpired by [element-resize-detector](https://github.com/wnr/element-resize-detector).

::: tip
You can open browser's dev-tool to adjust content's size and see the effect.
:::
<ClientOnly>
<Demo-Basic-DetectSizeChange />
</ClientOnly>

## 4.Pull-refresh or push-load supported

#### Vuescroll supports pull-refresh and push-load. It's uesful when you want to display a list of datas.

<ClientOnly>
<Demo-Basic-PullRefreshOrPushLoad />
</ClientOnly>

## 5.Paging

#### Vuescroll supports paging-mode. Well, It's userful when you want to show a carousel like [this](http://element-cn.eleme.io/#/zh-CN/component/carousel).

<ClientOnly>
<Demo-Basic-Paging />
</ClientOnly>

::: tip
To disable X or Y paging, just set scrollingY or X to false.

```javascript
ops: {
  scrollPanel: {
    scrollingY: false; // or scrollingX: false
  }
}
```

You had better to set your size of your each page to be equal to the size of the its parent dom, so that you won't see the content of another page in current view, that is to say , pnly show one page each time.
:::

## 6. Snapping

Vuescroll supports snapping while native doesn't. Snapping is similar to `Paging`, but there are alao a few difference: **Paging slides a full page each time, but snapping slides a user-defined distance each time**.

<ClientOnly>
<Demo-Basic-Snapping />
</ClientOnly>

## 7.Toggle between modes

#### You can even changes modes in runtime, and the postions won't be changed.

<ClientOnly>
<Demo-Basic-SwitchMode />
</ClientOnly>

::: warning
Perhaps not works well in mobile, becase slide and native are the same in mobile.
:::
