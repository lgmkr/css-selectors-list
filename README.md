## CSS Selectors list

#### Absolute evergreens
`*` - All elements are selected  
`.banana` - All elements with class banana selected  
`#banana` - All elements with id banana selected  
`p` - All `<p>` elements are selected  

#### Relative evergreens
`div, p` - All `<p>` and `<div>` elements are selected  
`div p` - Descendent selector. All `<p>` elements inside `<div>` elements are selected.  
`div > p` - Direct children. All `<p>` elements whose direct parent is `<div>` are selected. It works backwords too (`p < div`)  
`div + p` - All `<p>` elements places immediately after `<div>` element are selected.  
`div ~ p` - All `<p>` elements that are preceded by a `<div>` element are selected.  

#### Specific Category
##### This class is often used for attributes :target, title, lang and href.

`[title]` - All elements with the title attribute are selected.  
`[title=banana]` - All elements which have the 'banana' value of the title attribute.  
`[title~=banana]` - All elements which contain 'banana' in the value of the title attribute.  
`[title|=banana]` - All elements which value of the title attribute starts with 'banana'.  
`[title^=banana]` - All elements which value of the title attribute begins with 'banana'.  
`[title$=banana]` - All elements which value of the title attribute ends with 'banana'.  
`[title*=banana]` - All elements which value of the title attribute contains the substring 'banana'.  

### Quasi-Evergreens
##### These selectors are called **pseudo classes* and they must stay with other selector and describe it's state or property.

`:hover` - Selects elements when it is in the hover state.  
`:link` - Selects elements if they are links (once with href attribute).  
`:visited` - Selects elements if they have been visited.  
`:active` - Selects elements when they are active (clicked).  
`:focus` - Selects elements when they are focused.  
`:checked` - Selects elements when they are checked.  
`:required` - Selects elements with the required attribute.  
`:optional` - Selects elements without the required attribute.  
`:first-child` - Selects the first element within a parent.  
`:nth-child(number)` - Selects the child element based on a number (if it's 2 then selects second child, if it's 2n then selects all the children in steam positions).  
`:only-child` - Selects element only if it's the only child.  
`:first-of-type` - Selects the first element of the type.  
`:nth-of-type(number)` - Selects the child element of the type based on a number (if it's 2 then selects second of the type, if it's 2n then selects all children of the type in steam positions).  
`:only-of-type` - Selects element only if it's only of the type.  
`:empty` - Selects elements which contain no text or child elements.  

##### Pseudo elements 
`::before:` - Add content before the element (e.g. an opening quote, icon, image...).  
`::after` - Add content after the element (e.g. a closing quote, clearfix...).  
`::first-letter` - Selects the first letter of the element.  
`::first-line` - Selects the first line of the element.  
`::selection` - Selects a part of the element which is selected.
