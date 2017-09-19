# Horizontal Serverlist Plugin Addons
Here is a collection of my own creations to be used together with the **Horizontal Serverlist Plugin** *made by [square](https://github.com/Inve1951)*


## Black Pulsating Tooltips

### Preview
![](https://vgy.me/666ivb.gif) ![](https://vgy.me/htnABi.gif)
###### CSS Code
```css
/* Black pulsating tooltips */
.tooltip {
    background-color: #000000 !important;
    box-shadow: 0 0px 0px 0px, 0 0 0 2px var(--accent-color);
    padding: 9px 10px;
    border-radius: 10px;
    font-size: 14px;
    text-align: left;
    z-index: 1000000000000000000;
    pointer-events: none;
    animation: opacity 300ms linear, slide_up 200ms cubic-bezier(.1,1,0,1), text-pulse 2s ease infinite;
  }
@keyframes slide_up {
    from {
        transform: translate(0, 200%);
        }
    }
@keyframes text-pulse {
    20% {
        color:rgba(255,255,255,1);
    }
    40% {
        color:rgba(255,255,255,.6);
    }
    70% {
        color:rgba(255,255,255,1);
    }
    90% {
        color:rgba(255,255,255,.6);
    }
}
```
