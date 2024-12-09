# Social Scraping - ALPHA release

* Make sure you're registered and install our [extension](https://extension.blockmesh.xyz)

* Continue your regular social browsing, your extension will collect **public** data and earn points for you.
  (you will not see the points in your dashboard yet, this is coming in the next big update)

* If you want to earn more you can do the following:

1. Open a `tab` on Twitter.
2. Right click `inspect`.

![image](https://github.com/user-attachments/assets/80ebe2ad-67fc-4f95-b1b1-f67d2645f98c)

3. Paste the following code in the `console` , and leave it alone (we'll add this as a button in the extension next update).

```javascript
var scrollDistance = 800;
var interval = 4000;
var maxScrolls = null;
var scrollCount = 0;
var currentScrollPosition = window.pageYOffset || document.documentElement.scrollTop;
var scrollInterval = setInterval(function() {
    if (maxScrolls !== null && scrollCount >= maxScrolls) {
        clearInterval(scrollInterval);
        return;
    }
    currentScrollPosition += scrollDistance;
    window.scroll(0, currentScrollPosition);

    scrollCount++;
    console.log("scroll number", scrollCount);
}, interval);
```

## More Info

* We will post details on specific accounts with higher value.
  When we post about them, go to their profile and apply the script above and let it run in the background in a seperate tab.
  
* You can also use Twitter search for example to find older tweets:
  https://x.com/search?q=%28from%3A%40elonmusk%29+until%3A2023-02-01+since%3A2023-01-01&src=typed_query&f=top
