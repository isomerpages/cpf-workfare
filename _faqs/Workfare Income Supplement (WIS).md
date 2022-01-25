---
title: Workfare Income Supplement (WIS)
permalink: /faqs/WISFAQs
description: ""
---
[id^="togList"],                        /* HIDE CHECKBOX */
[id^="togList"] ~ .list,                /* HIDE LIST */
[id^="togList"] + label  span + span,   /* HIDE "Collapse" */
[id^="togList"]:checked + label span{   /* HIDE "Expand" (IF CHECKED) */
  display:none;
}
[id^="togList"]:checked + label span + span{
  display:inline-block;                 /* SHOW "Collapse" (IF CHECKED) */
}
[id^="togList"]:checked ~ .list{
  display:block;                        /* SHOW LIST (IF CHECKED) */
}

<div class="row">
  <input id="togList1" type="checkbox">
  <label for="togList1">
    <span>Expand</span>
    <span>Collapse</span>
  </label>
  <div class="list">
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
  </div>
</div>