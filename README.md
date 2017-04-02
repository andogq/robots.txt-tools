# robots.txt-tools
###### Because doesn't enjoy having a sniff around at robots.txt files?

---

### What is a robots.txt file?
- A file placed in the root of a website which requests pages for a web crawler to not index
- Goes along the lines of
```
	# robots.txt file for example.com
	User-agent: *
	Disallow: /not-indexed/*
	Allow: /not-indexed/indexed.html
```
- For more details [click here](https://support.google.com/webmasters/answer/6062608?hl=en&ref_topic=6061961)
 
---
 
### What is this script?
- This is a simple script which when loaded on a website, will load the site's robots.txt onto the page, with links to the files
- Can be used as a standalone script (`main.js`) or used as a bookmarklet (`main_bookmarklet.js`)
  - (only difference is that `main_bookmarklet` calls itself)

---

### How to use the script
1. Bookmark this page (or any page!) to your bookmarks bar
2. Edit the name of the bookmark to `robots.txt tools`
3. Change the url of the bookmark to:

	`javascript:(function(){document.body.appendChild(document.createElement('script')).src='https://rawgit.com/tom-ando/robots.txtTools/master/main_bookmarklet.js';})();`
4. That is it! Click the bookmark right now to test it