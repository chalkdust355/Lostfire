---
title: <%*  
let title = tp.file.title;
let attendee = await tp.system.prompt('Attendee: ');

if (title.startsWith('Untitled')) {  
  title = `${attendee}`; // Set and store the new title
  await tp.file.rename(title); 
}
-%><% title %>
draft: false
tags:
  - 
---