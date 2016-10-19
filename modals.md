---
layout: page
title: Modals
permalink: /modals/
group: "section"
order: 7
---

[Modals](http://semantic-ui.com/modules/modal.html#size) prevent users from interacting with the background while focusing on a specific task. For modals iLab uses a Semantic modal and the Magnific popup library. All new work should use the Semantic version.
Modals should be cancelled by three methods: (1) click a cancel button, (2) hit escape on the keyboard, (3) click outside of the modal on the window overlay.#### Code
The basic init for a [modal](http://semantic-ui.com/modules/modal.html#modal).

``` js
  $('.ui.modal')
    .modal()
  ;
```

#### Guidelines

- Place an X inside the upper right hand corner of the modal.
- [Size](http://semantic-ui.com/modules/modal.html#size) modals to the content. Use large for more details or image content. Use small for content usually placed in alerts (e.g., "Do you want to set your password?")
- Never change the animation or the background options (e.g., no blur).

*More guidelines:*

Apple provides [succinct guidance](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Modal.html) in it's iOS Human Interface Guidelines:

> Keep modal tasks simple, short, and narrowly focused. You don’t want your users to experience a modal view as a mini app within your app. If a subtask is too complex, people can lose sight of the main task they suspended when they entered the modal context. Be especially wary of creating a modal task that involves a hierarchy of views, because people can get lost and forget how to retrace their steps. If a modal task must contain subtasks in separate views, be sure to give users a single, clear path through the hierarchy, and avoid circularities. For guidelines on using modal views, see Modal View.

> Always provide an obvious and safe way to exit a modal task. People should always be able to predict the fate of their work when they dismiss a modal view.


