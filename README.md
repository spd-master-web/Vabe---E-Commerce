c# E-Commerce Redesign by VABÈ Team

Team members: Arianna V., Beatrice B.M., Elisa C., Vittoria F.

![Image of the team](https://github.com/spd-master-web/Vabe---E-Commerce/blob/main/team.jpg)

## Costa Del Mar

### Goal 01: Fix filters + view for the PLP

Create buttons to switch view.
1. Create a div container.
2. Insert buttons inside container.

```
jQuery("#slot-5").append("<div id='switchView'></div>");
jQuery("#switchView").html("<button id='btnSingle' type='button'>Single View</button><button id='btnDouble' type='button'>Gallery</button>");
```

Add grid and functions to buttons.
```
jQuery("#btnDouble").click(function() {jQuery("div.products-grid").addClass("gallery-view");});
jQuery("#btnSingle").click(function() {jQuery("div.products-grid").removeClass("gallery-view");});
jQuery("<style type='text/css'> .gallery-view{ display:grid; grid-template-columns:200px 200px;} </style>").appendTo("head");
```

Fix layout.
```
jQuery(".catEntryGrid_border").remove()
jQuery(".banner--vertical").css('grid-column', '1 / 3');
jQuery(".banner--vertical").css('order', '-10');
```

Quick check to see if button works (we may need it in the future):
```
jQuery("#btnSingle").click(function() {console.log("this working")});
```

Style buttons.
```
jQuery("#switchView").css('float', 'right');
```

## Sunglass Hut

### Goal 01: Fix filters for the PLP

The filter tab should be made more evident.

We changed the button color to highlight it.

```
$('.sgh-filters-actions--mobile').css('background-color', '#FF7714');
$('.sgh-filters-actions--mobile').css('color', '#FFF');
$('.sgh-filters-actions--mobile').css('border-color', 'transparent');
$('.sgh-filters-actions--mobile').css('text-transform', 'capitalize');
```

We worked on the icon by decoding it, changing the settings, and encoding it again.

```
.common__icon--filter-knobs {
  background-color: url("data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNSIgaGVpZ2h0PSIxNSIgdmlld0JveD0iMCAwIDE1IDE1Ij4KICA8ZyBmaWxsPSJub25lIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIHN0cm9rZT0iI2ZmZiIgc3Ryb2tlLXdpZHRoPSIuOCIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMSAxKSI+CiAgICA8cGF0aCBzdHJva2UtbGluZWNhcD0icm91bmQiIGQ9Ik0uODI0IDEuNzM5aDEyLjY0NE0uODI0IDYuNTg5aDEyLjY0NE0uODI0IDExLjQzOGgxMi42NDQiIC8+CiAgICA8Y2lyY2xlIGN4PSI5Ljg4MiIgY3k9IjEuNjQ3IiByPSIxLjY0NyIgZmlsbD0idHJhbnNwYXJlbnQiIC8+CiAgICA8Y2lyY2xlIGN4PSIxLjY0NyIgY3k9IjYuNTg4IiByPSIxLjY0NyIgZmlsbD0idHJhbnNwYXJlbnQiIC8+CiAgICA8Y2lyY2xlIGN4PSI3LjQxMiIgY3k9IjExLjUyOSIgcj0iMS42NDciIGZpbGw9InRyYW5zcGFyZW50IiAvPgogIDwvZz4KPC9zdmc+")
}
```

[Link to Encode](https://base64.guru/converter/encode/image/svg)

![Screenshot of the Updated Design](https://github.com/spd-master-web/Vabe---E-Commerce/blob/main/SGH/01_SGH/plp_filter.png)

### BRAVI TUTTI!
