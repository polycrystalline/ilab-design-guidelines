---
layout: page
title: Forms
permalink: /forms/
group: "section"
order: 6
---

[Forms](http://semantic-ui.com/collections/form.html) are an essential way users interact with iLab and they are how users achieve their goals. Therefore, iLab forms should be straightforward and fast to complete.
#### Code
Creating fields that are not the full width of the grid

``` haml
  .ui.form
    %h4.ui.header Reservation Time
    .fields
      .five.wide.field
        %label Minimum Minutes
        %input{:placeholder => "Min.", :type => "text"}
      / five wide field
      .five.wide.field
        %label Maximum Minutes
        %input{:placeholder => "Max.", :type => "text"}
      / five wide field
```



#### Guidelines
- Forms should be a single column, except for things like first name and last name or city and post code or other related data.

<div class="ui form">
  <h4 class="ui header">Reservation Time</h4>
  <div class="fields">
    <div class="five wide field">
        <label>Minimum Minutes</label>
        <input type="text" placeholder="Min.">
    </div> <!-- five wide field -->
    <div class="five wide field">
        <label>Maximum Minutes</label>
        <input type="text" placeholder="Max.">
    </div> <!-- five wide field -->
  </div>
</div>

- Avoid using sentences [in form labels](https://uxplanet.org/designing-more-efficient-forms-structure-inputs-labels-and-actions-e3a47007114f#.3db8lwnvg).
- Use help text to assist users in completing forms. Typically this should be placed in a popup.
- Use the [right case](https://developer.apple.com/library/mac/documentation/UserExperience/Conceptual/OSXHIGuidelines/TerminologyWording.html#//apple_ref/doc/uid/20000957-CH15-SW4)
  - Use Title Case for labels. For example: "Header Logo", "Header Height", "Tab Color"
- Checkboxes, toggles, and radio buttons may have labels that use sentence case, even if they are not complete sentences.
- Use a button labeled Back, since that is a normal way to interact with web applications.
- Avoid Cancel buttons.
- Never use [Reset buttons](https://www.nngroup.com/articles/reset-and-cancel-buttons/).

Reference: Here's some [excellent research and guidance](http://www.slideshare.net/cjforms/labels-and-buttons-on-forms) for buttons and labels on building good forms.


