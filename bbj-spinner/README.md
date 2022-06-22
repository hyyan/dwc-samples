# bbj-spinner

in BBj 22.02+ , DWC provides a spinner web component. A spinner provides a way to show the progress of an indeterminate operation.
The web component `<bbj-spinner>` API is documented [here](https://basishub.github.io/basis-next/#/dwc/bbj-spinner).

```Java
label! = "" +
: "<html>" +
: " <bbj-spinner style='margin-right: var(--bbj-space-s)'></bbj-spinner>" +
: " A Button with bbj-spinner" +
: "</html>" 
button! = window!.addButton(label!)
```

![button-with-spinner](https://user-images.githubusercontent.com/4313420/174987739-f17227ae-1316-4d96-8e3c-415a7fe45f3d.gif)
