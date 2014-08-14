polymer-date-picker
===================

A Polymer interpretation of Dan Grossman's awesome bootstrap-daterangepicker (https://github.com/dangrossman/bootstrap-daterangepicker)

![alt-text](https://raw.githubusercontent.com/christopheclc/polymer-date-picker/master/docs/images/datepicker-with-range.png "Example of polymer-date-picker with range")

## Usage
### Installation
```bash
bower install polyemr-date-picker
```

### Import
```html
<link rel="import" href="../polymer-date-picker/polymer-date-picker.html">
```

### Simple Date Picker
```html
<input id="trigger" value="{{selectedDate}}" 
  on-click="{{$.datePicker.toggle}}" 
  readonly class="date"/>
<polymer-date-picker 
  id="datePicker"
  selectedDate="{{selectedDate}}" 
  relatedTarget="{{$.trigger}}" 
  opened="false"/>
```
### Range
```html
<input id="triggerRange" 
  value="{{startDate}} to {{endDate}}" 
  on-click="{{$.datePicker.toggle}}" readonly/>
<polymer-date-picker 
  id="datePicker" 
  range 
  startDate="{{startDate}}" 
  endDate="{{endDate}}" 
  relatedTarget="{{$.triggerRange}}" 
  opened="false"/>
```

## Contributors
- Christophe Clapp
- Christopher Hartmann
