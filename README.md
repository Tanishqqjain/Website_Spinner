# Website_Spinner
Easy to use Spinner for websites, Which enables novice to insert spinner in their website without trouble.

-

> Alert Before using the below code first include (Bootstrap and Jquery files or CDNs)

## How to Use

#### Include the following code before `</body>` tag

```
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

