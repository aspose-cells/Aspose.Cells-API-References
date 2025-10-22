##PageEndSavingArgs
Info for a page ends saving process.
## PageEndSavingArgs class
Info for a page ends saving process.
```javascript
class PageEndSavingArgs extends PageSavingArgs;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(PageSavingArgs)](#constructor-pagesavingargs-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [hasMorePages](#hasMorePages--)| boolean | Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [pageIndex](#pageIndex--)| number | Readonly. Current page index, zero based. |
| [pageCount](#pageCount--)| number | Readonly. Total page count. |
### constructor(PageSavingArgs) {#constructor-pagesavingargs-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: PageSavingArgs);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PageSavingArgs | The parent object. |
### hasMorePages {#hasMorePages--}
Gets or sets a value indicating whether having more pages to be output. The default value is true.
```javascript
hasMorePages : boolean;
```
### pageIndex {#pageIndex--}
Readonly. Current page index, zero based.
```javascript
pageIndex : number;
```
### pageCount {#pageCount--}
Readonly. Total page count.
```javascript
pageCount : number;
```
