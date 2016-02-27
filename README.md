# nodecg-hue
> WIP NodeCG bundle to control Philips Hue lighting system

## Extra Usage Steps
Change directories to ```bundles/nodecg-hue``` and run the following command
```
browserify dashboard/panel.js -o panel-browserified.js
```

## Todo
### Short Term
- add warning when updating lights when no lights have been selected
- ability to shift bri, hue, sat
- stop sliders with large input values from being visually cut off
- update color-preview on color-picker tab change
- make finding and connecting to hue bridge robust
- add message to background of light selection div while waiting to find lights/groups
- implement a search for new lights feature
- implement light scheduling - [schedules API](http://www.developers.meethue.com/documentation/schedules-api-0)
- create a settings dialog that contains rarely changed lightstate options (bridge name, proxy port, touchlink, netmask, gateway)
- create a settings element on the panel that contains frequently changed lightstate options (color effect)

### Long Term
- create a visual color picker with the ability to save favourite colors
- consider moving scenes to a separate panel
- add ability to select from a couple different layout designs
- look into light rules - [rules API](http://www.developers.meethue.com/documentation/rules-api)
- look into light sensors - [sensors API](http://www.developers.meethue.com/documentation/supported-sensors)
- gain better understanding of Polymer to see if there is a better way to track slider value changes than attaching a boatload eventListeners
- consider making a Polymer element out of the color picker
- consider using [tinycolor2](https://www.npmjs.com/package/tinycolor2) or other color manipulation library
- create extension API with documentation
- make bundle production ready (minimize js/css, figure out best building solution)


*some links require Philips Hue API login
