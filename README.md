

_<p align="center">"Eating website for fun... nyom nyom nyom"</p>_

<div align="center" style="text-align:center; margin:auto;">
<img align="center" src="https://i.imgur.com/EgCvXyK.png" width="150"/>
</div>


```javascript
const tabItems = document.querySelectorAll(".tab-item");
const tabContentItems = document.querySelectorAll(".tab-content-item");

// Select tab content
function selectItem(e) {
  removeBorder();
  removeShow();
  // Add border to current tab
  this.classList.add("tab-border");
  // Grab content item from DOM
  const tabContentItem = document.querySelector(`#${this.id}-content`);
  // Add show class
  tabContentItem.classList.add("show");
}
function removeBorder() {
  tabItems.forEach(item => item.classList.remove("tab-border"));
}
function removeShow() {
  tabContentItems.forEach(item => item.classList.remove("show"));
}
// Listen for tab click
tabItems.forEach(item => item.addEventListener("click", selectItem));
```



```html
<!-- Content Pretty Long so I'll add later -->
<!-- But this is the basic gist -->
<div class="tab-item">
  <!-- Selectors for the different tab content -->
</div>
<div class="tab-content-item">
  <!-- Content of each tab item -->
</div>
<!-- Simply add more selectors and corresponding 
tab content for each selector -->
```

