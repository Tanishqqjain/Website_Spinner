# Website_Spinner

 Easy to use Spinner for websites, Which enables novice to insert spinner in their website without trouble.

> Alert Before using the below code first include **(Bootstrap and Jquery files or CDNs)**

- [Boostrap CDN](https://getbootstrap.com/docs/4.0/getting-started/introduction/)
- [Jquery CDN](https://code.jquery.com/)

## How to Use

#### Include the following code before `</body>` tag

``` HTML
<div class="w-100 " style="height: 100% !important; position: fixed; display: flex; justify-content: center; align-items: center; z-index: 99999; background-color: rgba(0, 0, 0, 0.5); top: 0; left: 0; color:mintcream;" id="spinner">
    <div class="spinner-border" role="status">
        <span class="sr-only">Loading...</span>
    </div>
</div>
```

#### Enable the Spinner

`$('#spinner').fadeIn("slow");`

#### Disable the Spinner

`$('#spinner').fadeOut("slow");`

## Some Useful Examples =>

#### 1. )) when Page is completely loaded then hide the spinner

``` JavaScript
    <script>
        $(window).on('load', function(){
            $('#spinner').fadeOut("slow");
        });
    </script>
```

#### 2. )) when an element (id="btn1") is clicked then show spinner

``` JavaScript
    <script>
        $('#btn1').on('click', function(){
            $('#spinner').fadeIn("slow");
        });
    </script>
```

#### 3. )) When an anchor tag a link is clicked then first Enable the Spinner and then move to specified page.

- Step1:  Convert the `<a>` tag to `<div>` tag

- Step2:  Add the following attribute _(Replace "newPage.html" --> "href_link.html")_

    ``` HTML
    onClick="(function(){ $('#spinner').fadeIn("fast"); window.location.href = "newPage.html"; })();"
    ```

- An example is shown below :

    ``` HTML
    <a href="name1.html" >Click me</a>

                👇🏻👇🏻👇🏻

    <div onClick="(function(){ $('#spinner').fadeIn("fast"); window.location.href = "name1.html"; })();" >Click me</div>

    ```
