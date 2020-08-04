# angular-tooltip-directive


A simple tooltip directive which can be used in Angular application in any HTML element to render tooltip.

### Installation
You can download `tooltip.directive.ts` and `tooltip.scss` files into your Angular project, then all you need to declare `TooltipDirective` in your app.module.ts or any shared or feature level module.

```typescript
@NgModule({
  declarations: [
    TooltipDirective
  ],
  imports: [...],
  providers: [...],
  bootstrap: [...]
})
```

And import tooptip css into root `styles.scss` file to use it globally.

```scss
@import 'tooltip';
```

### Input Options
* **tooltip:** tooltip text which will show as tooltip
* **delay:** show hide tooltip with delay animation i.e `1000`milliseconds
* **placement:** the placement of tooltip to show, `bottom`, `top`, `left`, `right` default is `bottom`


### Usage
```html
Tooltip with default options
<a 
   href="https://google.com" 
   tooltip="Put your tooltip text here">
   This is tooltip with default placement
</a>

Tooltip with placement top
<p 
   placement="top"
   tooltip="Put your tooltip text here">
   This is tooltip with placement top
</p>

Tooltip with placement left
<a 
   href="https://google.com" 
   placement="left"
   tooltip="Put your tooltip text here">
   This is tooltip with placement left
</a>

Tooltip with placement right
<a 
   href="https://google.com" 
   placement="right"
   tooltip="Put your tooltip text here">
   This is tooltip with placement right
</a>

Tooltip with delay 
<button 
   type="button" 
   [delay]=1000
   tooltip="Put your tooltip text here">
   This is tooltip show with delay
</button>
```

