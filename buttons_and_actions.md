---
layout: page
title: Buttons & Actions
permalink: /buttons-and-actions/
group: "section"
order: 2
---

Buttons are to take actions on a form or other work.

#### Code

	%button.ui.black.basic.button.cancel
	  Back
	%button.ui.primary.button
	  Create Item

#### Guidelines
- The primary button should be colored (i.e., high contrast).
- The action that advances the users goal, usually a positive, primary action, the most should be the furthest right.

<button class="ui black basic button cancel">
  Back
</button>
<button class="ui primary button">
  Create Item
</button>

- Actions should be grouped together to the right of the content, without being orphaned.
- Use title case as elaborated by the [OSX spec](https://developer.apple.com/library/mac/documentation/UserExperience/Conceptual/OSXHIGuidelines/TerminologyWording.html#//apple_ref/doc/uid/20000957-CH15-SW4)
- Secondary buttons should be [basic](http://semantic-ui.com/elements/button.html#basic) or links.
- Avoid using the standard button style. In a few usability tests, users have said that the button looks disabled.

<div class="ui button">
  Avoid this Button
</div>
- Avoid using the conditional button. The conditional button lacks visual distinction between the primary and secondary action.
<div class="ui buttons">
  <button class="ui negative button">Neither</button>
  <div class="or"></div>
  <button class="ui primary button">Nor</button>
</div>

#### Button Color and Styling Guidelines
Using the conventional and consistent button [colors and styling](http://uxmovement.com/buttons/how-button-color-contrast-guides-users-to-action/) speeds a user's work and prevents mistakes. First, identify what type of action button is taking:

- Positive: updates, sends or adds information.
- Positive plus redirect to new page.
- Neutral: makes no changes or goes back
- Negative: delete, destroy, remove or block information.

Second, identify the primary action:

- Usually the primary action is the positive action. 
- When positive and negative actions are together, make the positive the primary.

**Make the primary action the highest contrast and most prominent, placed furthest to the right.**

<button class="ui red basic button">
  Negative
</button>
<button class="ui primary button">Positive</button><i class="checkmark icon"></i>

<button class="ui black basic button">
  Neutral
</button>
<button class="ui negative button">Negative</button><i class="checkmark icon"></i>

<button class="ui black basic button">
  Neutral
</button>
<button class="ui red basic button">
  Negative
</button>
<button class="ui primary button">Positive</button><i class="checkmark icon"></i>

Reserve green for when a user will be redirected after taking the positive action.

<button class="ui black basic button">
  Back
</button>
<button class="ui red basic button">
  Remove Session
</button>
<button class="ui blue basic button">
  Start Session
</button>
<button class="ui green button">
  Start Session and Logout
</button><i class="checkmark icon"></i>
