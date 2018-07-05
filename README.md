jQuery-Visibly
==============

A jQuery Plugin designed to easily show elements based on values of other elements

## Documentation

### Setup
```javascript
$('[visibly]').Visibly();
```


### Options
```javascript
clearOnHide: false,  //Clear the data from the elements on hide
regularExpression: false, //This determines if regular expression is to be used for the test
attr: 'visibly', //Data attribute to use for the visibly data
vdelim: ',', //Delimeter used to split the values a control can hold
edelim: ':', //Delimeter between the field ID and the values
fdelim: ';' //Delimeter between the fields
rdelim: '%' //Delimeter between the rules
cssSelector: false //use css selector to select value source instead of input name or id selector eg ".className:value"

```

## Examples

``` 
<div visibly="field1:a,b;field2:1"></div> 
```
The above rule will make the relevant element visible is the value of field1 is either 'a' or 'b' and field2 has value of '1'


## Examples

# Using cssSelector : true option
``` 
<select class="source">
	  <option value="-1">-1</option>
	  <option value="0">0</option>
	  <option value="1">1</option>
	  <option value="2">2</option>
</select>
<div visibly=".source:0,1;"></div>
```
The above rule will make the relevant element visible is the value of .source is either '0' or '1'


## Help
Full documentation can be found at: http://www.danielrivers.com/visibly