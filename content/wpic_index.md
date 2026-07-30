
---
title: "Welcome to my site"
---

![myphoto](/me_photo.png?width=50px&height=50px) 
![myphoto](/me_photo.jpeg?width=50px&height=50px) 
Hi, I'm Clint Reyes, a PhD student in Ocean Engineering. \
You can find more about me and my research on this page.  

{{ $image := .Resources.Get "me_photo.jpeg" }}

{{ $image := .Resources.GetMatch "me_photo.jpeg" }}
<img src="{{ $image.RelPermalink }}" width="{{ $image.Width }}" height="{{ $image.Height }}">

{{ $image := resources.Get "images/me_photo.jpeg" }}

![alt](me_photo.jpeg "=350x")