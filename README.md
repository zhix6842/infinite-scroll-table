# Infinite Scroll Table

This is a Infinite Scroll Table Unit

## Getting Started

You Need a Backend webService and you can use it

### Install

It Need Jquery

```
<script src="https://code.jquery.com/jquery-1.12.4.min.js" integrity="sha256-ZosEbRLbNQzLpnKIkEdrPv7lOy9C27hHQ+Xp8a4MxAQ=" crossorigin="anonymous"></script>
<script src="t4u.Scroll.js"></script>
```

### Usage


```
var titleModel = [
				{ display: 'id', name: 'f_id', width: 45, sortable: false, align: 'center' },
				{ display: 'name', name: 'f_first_name', width: 50, sortable: false, align: 'left' },
				{ display: 'address Company', name: 'f_address', width: 140, sortable: false, align: 'left' },
				{ display: 'birthday', name: 'f_birthday', width: 140, sortable: false, align: 'left' },
				{ display: 'Setup Date', name: 'f_post_time', width: 120, sortable: false, align: 'left' }
			];
var contentModel = [];
$(window).t4uInfiniteScroll({
				url: "http://localhost:2751/NewsFeed/NextPage", //ajax url
				selector: ".table-content", //table
				titleModel: titleModel, // table th
				contentModel: contentModel, //table content
				rp: 20, 
				sort: "f_id", //sort
				sortorder: "asc", // sort method
			});
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

