---
layout: page
title: Visual Design
permalink: /visual_design/
---

# iLab Design Guidelines

The iLab Design Guidelines are intended to create a uniform and intuitive standard for design. This guide will not solve every problem, but should serve as starting point to decision making.

## Visual Design

### Typography
Typography heavily influences usability.

#### Code


	body {
	  ...
	  font-family: Lato,'Helvetica Neue',Arial,Helvetica,sans-serif;
	  font-size: 14px;
	  ...
	}


#### Guidelines


- Use a base font size from semantic 14px for paragraph fonts. All other fonts should be scaled from this with rem or em.
- Use the default sans serif fonts in the Semantic package.
- iLab does not currently support multiple font styles and they should be avoided.
- A line 66 characters long, counting spaces characters and is generally considered the optimal size for a line’s length.

### Capitalization
Use [consistent capitalization](https://www.nngroup.com/articles/113-design-guidelines-homepage-usability/). Capitalization conveys meaning (e.g., importance). Inconsistencies like capitalization can disorient users.

These are general guidelines for text within the app.

#### Guidelines
- Use sentence case when the text is a complete sentence (subject + predicate/verb + full stop punctuation). 
  - Sentences should be used to provide assistance to users.
- Use title case for headers, actions and labels.
- Avoid use of all caps because it slows down users making text difficult to read.
- Avoid use of all lowercase because it does not tell the user what is important and what is less important.

### Currency
Many of iLab's views include financial information. Financial users have conventions for displaying currency and financial data that iLab should support.


#### Guidelines
- For USD, EUR, GBP, CAD, AUD and CHF, there should always be two digits after the radix (i.e., decimal point). Secondarily, European or other international users should be able to swap the radix and display of comma and decimal point delimiters. Currencies should always be preceded by their symbol $, €, even if a subtotal.
- For some currencies, that may not have a symbol like Norwegian krone, the label should be after.
- When calculating the items total cost, call the column with the calculated value "Amount".
- For some currencies, their should be no space between the symbol.
- For tables that have currencies, the table heading and the values should be right aligned, so that the decimal points are aligned.

### Date Formats
Dates should be in the default format, ideally by user selected but potentially organizationally determined or at least defined by the locale.Dates can take different formats in different contexts. For example, within the context of a weekly calendar, the date in the day’s column heading may be shortened to either Mon 3/14 or Mon 14/3.

#### Code

|    Code    |         Example      |          Label         |
|------------|----------------------|------------------------|
| yyyy/mm/dd |      2020/10/04      | ISO, default           |
| mm/dd/yyyy |      10/04/2020      | US, default            |
| dd/mm/yyyy |      04/10/2020      | International, default |
| %m %d      | Oct 4                | US/Intl., short        |
| %m %d      | Wed 15/12, Wed 12/15 | US/Intl. calendar      |
| %l:%M %p   | 4:41 AM, 4:42 PM     |                        |
| %h:%M      | 4:41, 16:42          |                        |

#### Guidelines
- Use the core's timezone by default.

### Alignment

#### Guidelines
- Avoid adjusting the indentation (e.g., padding-left)that is built into Semantic UI's CSS.
- Text should be left aligned, except in cases of tables (e.g., currency) and marketing.

### Color
Use grayscale first. After that, add one color to add focus. Add additional colors at your own peril.
#### Design Palette

To match iLab's enterprise-wide styling, please use the following colors. Please note that we are using the default colors from the [Semantic UI library](http://semantic-ui.com/introduction/getting-started.html) for most buttons.

| Name                      | | Hex Code | Swatch |
|---------------------------|-|----------|--------|
| iLab Blue (main color)    | | #548DD4  | ![image](file:///Users/jtholden/Desktop/iLab/Guidelines/images/blue-ilab.svg) |
| Darker Blue               | | #376092  | ![image](file:///Users/jtholden/Desktop/iLab/Guidelines/images/blue-steel.svg) |
| Darker Grey               | | #777777  | ![image](file:///Users/jtholden/Desktop/iLab/Guidelines/images/gray-dark.svg) |
| Highlight Orange          | | #FA7921  | ![image](file:///Users/jtholden/Desktop/iLab/Guidelines/images/orange-dutch.svg) |
| Highlight/Background Grey | | #CCCCCC  | ![image](file:///Users/jtholden/Desktop/iLab/Guidelines/images/blue-ilab.svg) |
| Dark Grey for Font        | | #222222  | ![image](file:///Users/jtholden/Desktop/iLab/Guidelines/images/black-sky.svg) |


### Accessibility

We must take accessibility into account when designing and developing interfaces. iLab is reviewing the U.S. Governments [Section 508 Standards](http://www.section508.gov/content/learn/standards) as a potential guideline.

### Breadcrumbs
Use breadcrumbs to help give users a sense of where they are in iLab and help then navigate back and sideways.

![image](file:/images/breadcrumbs-example.png)

