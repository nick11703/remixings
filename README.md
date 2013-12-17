remixins for {less}
-
###Automatically convert pixel measures into rem units.

remixins is a collection of **{less}** mixins that helps you start using rem units without coding pixels fallbacks on every rule. Code your CSS using pixels. remixins will automatically convert them to rem units.

remixins includes **{less}** mixins for most popular properties where rem is used as a measure unit.

All non pixel values will be ignored so you can pass values when using css shorthand. examples and cheat sheet are included at top of less file.

Mixins available for the following CSS properties:  
 * FONTS: `font-size`, `line-height`, `text-indent` and `letter-spacing`
 * BORDERS & OUTLINES: `border-size`, `border` and `outline`
 * BORDER RADIUS: `border-radius`
 * MARGINS: `margin`(s)
 * PADDINGS: `padding`(s)
 * HEIGHTS & WIDTHS: `height` and `width` (including min- and max-)
 * POSITIONING: `top`, `left`, `bottom` and `right`
 * BACKGROUNDS: `background-size`, `background`
 * SHADOWS: `box-shadow` and `text-shadow`

#### How to use it:
1. Download remixins.less
2. Set `@baseValue` (line 95) to your integer root's font size. Note that `@baseValue` **MUST BE AN INTEGER** (without any measure unit).
3. Import downloaded file `@import "remixins.less`.

### Examples:
**{less}:**  
```css
    .element {
        .font-size(16px);
    }
```  
**CSS result:**  
```css
    .element {
        font-size: 16px;
        font-size: 1.6rem;
    }
```

**{less}**  
```css
    .element {
        .margin(10px, 3%);
    }
```  
**CSS result:**  
```css 
    .element {
        margin: 10px 3%;
        margin: 1rem 3%;
    }
```

### Included mixins
* `.font-size(@value)`
* `.line-height(@value)`
* `.text-indent(@value)`
* `.letter-spacing(@value)`
* `.border-size(@value)`
* `.border(...)`
* `.border-top(@value)`
* `.border-bottom(@value)`
* `.border-left(@value)`
* `.border-right(@value)`
* `.outline(...)`
* `.outline-width(@value)`
* `.border-radius(...)`
* `.border-top-left-radius(@value)`
* `.border-top-right-radius(@value)`
* `.border-bottom-left-radius(@value)`
* `.border-bottom-right-radius(@value)`
* `.margin(...)`
* `.margin-top(@value)`
* `.margin-right(@value)`
* `.margin-bottom(@value)`
* `.margin-left(@value)`
* `.padding(...)`
* `.padding-top(@value)`
* `.padding-right(@value)`
* `.padding-bottom(@value)`
* `.padding-left(@value)`
* `.height(@value)`
* `.min-height(@value)`
* `.max-height(@value)`
* `.width(@value)`
* `.min-width(@value)`
* `.max-width(@value)`
* `.top(@value)`
* `.left(@value)`
* `.bottom(@value)`
* `.right(@value)`
* `.background-size(...)`
* `.background(...)`
* `.box-shadow(...)`
* `.text-shadow(...)`

**@nick11703**
**@kaseybon**
