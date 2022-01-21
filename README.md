# Sidebery-CSS-tweaks
My CSS for Sidebery - sidebar and groups, with red gradient theme.

## Begin sidebar
```
/* sidebar */

#root {
  --tabs-height: 42px !important;
  --tabs-title-padding: 10px;
  --tabs-title-lines: 2;
}

.Tab .t-box {
  align-items: left;
  max-height: calc(var(--tabs-height) - var(--tabs-title-padding));
  overflow: hidden;
}

.Tab .title {
  font-size: var(--tabs-font-size);
  white-space: pre-wrap;
  line-height: calc((var(--tabs-height) - var(--tabs-title-padding)) / var(--tabs-title-lines));
}

.Tab[data-parent="true"] .title {
  font-size: 16px;
  font-weight: bold;
  --tabs-height: 44px !important;
}
```
## Begin groups page
```
/* group page */

#body {
  --bg-size: 0px 0px;
  --bg-img: url("");
}

#title {
  $font-family: 'cursive';
  margin: 0;
  font-size: 5em;
  margin-top: .5em;
  margin-bottom: .5em;
  color: black;
  text-shadow: 0 0 0.05em #fff, 0 0 0.2em #f2951b, 0 0 0.3em #ff0000;
  transform: rotate(-7deg);
}

#tabs .tab {
  height: 300px;
}

#tabs .bg {
  height: 200px;
  opacity: 1;
  position: unset;
}

.tab-title {
  background: linear-gradient(
    to right, 
    hsl(420 100% 62%), 
    hsl(350 100% 59%)
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  text-align: center;
}

.tab-url {
  color: #c4c4c4;
}

.fav-placeholder {
  height: 30px;
  width: 30px;
}

.fav {
  height: 30px;
  width: 30px;
}
```

![Sample Groups Tab Page](/assets/images/sidebery-groups-page.jpg)
