# L.Control.BootstrapModal

A simple Leaflet control to open a Bootstrap modal.

Modals are great for help panels, or for feedback forms, or for displaying a legend that doesn't need to take up screen space all the time. And if you want a Leaflet-styled button on your map, which would trigger this modal... here's the plugin for you.

# Usage

For a quick start, see the *example* folder, or the live demo: http://gregallensworth.github.io/L.Control.BootstrapModal/

Assuming that you already have a Bootstrap modal set up on your page, and already have a Leaflet map running, the control runs like this:

```
new L.Control.BootstrapModal({
    modalId: 'modal_help',
    tooltip: "How to use this thing",
    glyph: 'question-sign'
}).addTo(MAP);
```

Parameters are:

* **modalId** -- The DOM ID of the modal, e.g. what you put inside the id="" part. **Required**

* **tooltip** -- A tooltip to be displayed when the user hovers their mouse over the button. **Optional**

* **glyph** -- Which of the Bootstrap Glyphicons to display in the button. See http://getbootstrap.com/components/#glyphicons for the full list. **Optional** and defaults to a "i" icon.

