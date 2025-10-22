##PdfBookmarkEntry
PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or  current instance will be hidden and children will be inserted on current level.
## PdfBookmarkEntry class
PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or "", current instance will be hidden and children will be inserted on current level.
```javascript
class PdfBookmarkEntry;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [text](#text--)| string | Title of a bookmark. |
| [destination](#destination--)| Cell | The cell to which the bookmark link. |
| [destinationName](#destinationName--)| string | Gets or sets name of destination. |
| [isOpen](#isOpen--)| boolean | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [isCollapse](#isCollapse--)| boolean | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### text {#text--}
Title of a bookmark.
```javascript
text : string;
```
### destination {#destination--}
The cell to which the bookmark link.
```javascript
destination : Cell;
```
### destinationName {#destinationName--}
Gets or sets name of destination.
```javascript
destinationName : string;
```
**Remarks**
If destination name is set, the destination will be defined as a named destination with this name.
### isOpen {#isOpen--}
When this property is true, the bookmarkentry will expand, otherwise it will collapse.
```javascript
isOpen : boolean;
```
### isCollapse {#isCollapse--}
When this property is true, the bookmarkentry will collapse, otherwise it will expand.
```javascript
isCollapse : boolean;
```
