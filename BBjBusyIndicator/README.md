# BBjBusyIndicator

in BBj 22.02+ , a custom web component for the `BBjBusyIndicator` has been implemented. 
The web component `<bbj-busy>` API is documented [here](https://basishub.github.io/basis-next/#/dwc/bbj-busy).

BBjBusyIndicator depends on the following components:

* [bbj-backdrop](https://basishub.github.io/basis-next/#/dwc/bbj-backdrop)
* [bbj-spinner](https://basishub.github.io/basis-next/#/dwc/bbj-spinner)

```Java
  busy! = BBjAPI().getBuiManager().getBusyIndicator(err=*return)
  busy!.setText("The busy indicator is running ...")
  
  busy!.setAttribute("spinner-clockwise", "false")
  busy!.setAttribute("spinner-speed", "2000")
  busy!.setAttribute("spinner-theme", "danger")

  busy!.setVisible(1)
  wait 3

  busy!.setText("The busy indicator is running with the 'warning' theme ...")
  busy!.setAttribute("spinner-theme","warning")
  wait 3

  busy!.setText("All done and the 'success' theme is activated ...")
  busy!.setAttribute("spinner-theme","success")
  wait 2

  busy!.setVisible(0)
```

![BusyIndicator](https://user-images.githubusercontent.com/4313420/174982194-90a589ff-02ce-47bb-b416-779e3615a5bb.gif)


