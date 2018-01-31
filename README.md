# D3 tooltip

## See the [Project Page](https://bumbeishvili.github.io/d3-tooltip/) for interactive example!


## See usage example [at this codepen](https://codepen.io/bumbeishvili/pen/WMvNxM?editors=1010)

## screenshot
![image](assets/scr.png)

### Highlights
* Dynamic resizing
* High number of customization options

### Usage
1. Include `tooltip.js` file into you app

```html
 <script src="tooltip.js"></script>
```
2. Initialize tooltip inside your d3 visual

```javascript
 var tooltip = d3.componentsTooltip()
        .container('.svg-element')
        .content([
          {
            left: "default id",
            right: "{id}"
          },
          {
            left: "default value",
            right: "{value}"
          },
        ])
```

3. Show or hide it on your events
```javascript
   // show tooltip
        tooltip
        .x(100)
        .y(100)
        .show({id:1,value:"some value",name:"some large name"})
```

```javascript
//hide
tooltip.hide()
```
