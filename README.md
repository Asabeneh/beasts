Tips to responsive web design on a layout, 

create a layout containing: 
    - scalable fluid media e.g images
    - scalable typography 
    - lazy loading (if possible)


## Responsive Web Design(RWD) Tips 

These are some steps to achieve responsive elements for your layout 

## Images
*  use ``` srcset="" ``` **optimized image sizes**

```
<img src="./image.jpg" 

    <!-- alternative image sizes --->
    
    srcset="image-350.jpg 200w,
    image-500.jpg 500w,
    image-2000.jpg 1024w"

alt="an image"> 
```

## Typography

At the ```root``` of the document, 
create default font properties e.g.

```
    html, body { 
        font-size: 16px;
    } 

    p { 
        font-size: 0.5rem; /* 8px */
        
    /*
    use rem |or| (root)em's >> 

    rem: requires on font-size, set
    by default in most browsers 

    */

    }
```

## Media Queries 

Re-write styles for your layout depending on the screen-width measured by the vw(viewport-width)

```
/* small screens */
@media only and (max-width:480px) { 
   
    /*
         for >> small screens
         // code layout-styles
    */
}

@media only and (max-width:580px) { 

    /*
          for >> medium screens
          // code layout-styles 
     */

}

@media only and (max-width:980px) { 

    /*
          for >> large screens  
         // code layout-styles
     */
}
```

## Grids & Flex
Furthermore, table layouts can be stacked vertically(columns) or horizontally(rows), 

css grid & flexBox are two solutions when combined, provide a dynamic layout, also known as (a.k.a) responsive layout.


```
    <!--HTML--->
    <div class="parent-element>
        <div class="child-element"></div>
    </div>
   
    parent-element { 
        /* css */
        display: grid |or| flex;
        
        /*  css-grid  */
        grid-template-auto: row || column;
        
       /*  flex-box */
        flex-direction: row || column;

    }

```

# GoodLuck !
@evans 2019