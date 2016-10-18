---
layout: page
title: Tables
permalink: /tables/
order: 5
---


[Tables](http://semantic-ui.com/collections/table.html#single-line) are best for organizing structured datasets where each row represents a record.
#### Code
A basic striped table

```haml
%table.ui.striped.table
  %thead
    %tr
      %th Item
      %th Description
      %th.right.aligned Qty
      %th.right.aligned Unit Price
      %th.right.aligned Amount
  %tbody
    %tr
      %td Scans
      %td CT Scan
      %td.right.aligned 20
      %td.right.aligned 30.00
      %td.right.aligned 600.00
```		
You may also include a footer that includes information like a total or summary.

```haml
%tfoot
  %tr
    %th 3 People
    %th 2 Approved
    %th
```	  
Here's the CSS to make rows hover-able

```css
tr i.fa-pencil-square-o {
   visibility: hidden;
}
tr:hover i.fa-pencil-square-o {
   visibility: visible;
}
```

#### Guidelines
- Tables should be minimally responsive or scrollable for small widths.
- Actions on a table row should not be visible unless the row is hovered by a user.

![image]({{ site.baseurl }}/images/table-show-button.gif)

- Use the datatables.net filter 
- Zebra-striping tables is OK. [Research][zebra] indicates that zebra striping does not improve speed or accuracy of answering questions with data, although users do indicate an aesthetic preference for zebra striping.
- Never use the ribbon label `class="ui ribbon label"`

[zebra]: http://alistapart.com/article/zebrastripingmoredataforthecase

<table class="ui striped table">
  <thead>
    <tr>
      <th>Item</th>
      <th>Description</th>
      <th class="right aligned">Qty</th>
      <th class="right aligned" >Unit Price</th>
      <th class="right aligned">Amount</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Scans</td>
      <td>CT Scan</td>
      <td class="right aligned">20</td>
      <td class="right aligned">30.00</td>
      <td class="right aligned">600.00</td>
    </tr>
    <tr>
      <td>Scans</td>
      <td>MRI</td>
      <td class="right aligned">20</td>
      <td class="right aligned">30.00</td>
      <td class="right aligned">600.00</td>
    </tr>
    <tr>
      <td>Services</td>
      <td>Scans Services</td>
      <td class="right aligned">5</td>
      <td class="right aligned">50.00</td>
      <td class="right aligned">250.00</td>
    </tr>
    <tr>
      <td>Services</td>
      <td>Scans Services</td>
      <td class="right aligned">5</td>
      <td class="right aligned">50.00</td>
      <td class="right aligned">250.00</td>
    </tr>
    <tr>
      <td>Services</td>
      <td>Scans Services</td>
      <td class="right aligned">5</td>
      <td class="right aligned">50.00</td>
      <td class="right aligned">250.00</td>
    </tr>
    <tr>
      <td>Services</td>
      <td>Scans Services</td>
      <td class="right aligned">5</td>
      <td class="right aligned">50.00</td>
      <td class="right aligned">250.00</td>
    </tr>
    <tr>
      <td>Services</td>
      <td>Scans Services</td>
      <td class="right aligned">5</td>
      <td class="right aligned">50.00</td>
      <td class="right aligned">250.00</td>
    </tr>
    <tr>
      <td>Services</td>
      <td>Scans Services</td>
      <td class="right aligned">5</td>
      <td class="right aligned">50.00</td>
      <td class="right aligned">250.00</td>
    </tr>
  </tbody>
  <tfoot>
  <tr>
    <th colspan="4" class="right aligned">
      <strong>Grand Total</strong>
    </th>
    <th class="right aligned">
      <strong>$2700.00</strong>
  </th>
  </tfoot>
</table>


