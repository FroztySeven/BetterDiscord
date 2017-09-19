# Horizontal Serverlist Plugin Addons
Here is a collection of my own creations to be used together with the **Horizontal Serverlist Plugin** *made by [square](https://github.com/Inve1951)*
**__NOTICE: CSS Codes on this document will not work properly without the Horizontal Serverlist Plugin ✖__**
**__NOTICE: CSS Codes on this document should work with any themes ✓__**


## Black Pulsating Serverlist Tooltips - v1.0
*If you don't like the pulse effect on the tooltip, remove everything containing "text-pulse"*

### Preview
![](https://vgy.me/6vHGvp.gif)
###### Full CSS Code
```css
/* Black pulsating horizontal serverlist tooltips */
  .tooltip.tooltip-right.tooltip-black {
    background-color: #000000 !important;
    transform: translate(-119px, -72px) !important;
    width: 150px;
    padding: 13px;
    border-radius: 10px;
    font-size: 14px;
    text-align: center;
    z-index: 1000000000000000000;
    pointer-events: none;
    animation: opacity 300ms linear, slide_up 200ms cubic-bezier(.1,1,0,1), text-pulse 2s ease infinite;
  }
/* Black pulsating horizontal serverlist tooltip for Direct Messages */
  .guilds-wrapper .guilds .guild .guild-inner a {
    width:180%;
    height:100%;
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
## Accent Color Box-Shadow (Mini-enhancement)
### Preview
![](https://vgy.me/uwqtDz.gif)
###### Add this inside section ".tooltip.tooltip-right.tooltip-black {"
```css
    box-shadow: 0 0px 0px 0px, 0 0 0 2px var(--accent-color)!important;
