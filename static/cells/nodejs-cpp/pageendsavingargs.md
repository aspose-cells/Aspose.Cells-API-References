##PageEndSavingArgs
Info for a page ends saving process.
## PageEndSavingArgs class
Info for a page ends saving process.
```javascript
class PageEndSavingArgs extends PageSavingArgs;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(PageSavingArgs)](#constructor-pagesavingargs-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [hasMorePages](#hasMorePages--)| boolean | Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [pageIndex](#pageIndex--)| number | Readonly. Current page index, zero based. |
| [pageCount](#pageCount--)| number | Readonly. Total page count. |
## Methods
| Method | Description |
| --- | --- |
| [getHasMorePages()](#getHasMorePages--)| <b>@deprecated.</b> Please use the 'hasMorePages' property instead. Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [setHasMorePages(boolean)](#setHasMorePages-boolean-)| <b>@deprecated.</b> Please use the 'hasMorePages' property instead. Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getPageIndex()](#getPageIndex--)| <b>@deprecated.</b> Please use the 'pageIndex' property instead. Current page index, zero based. |
| [getPageCount()](#getPageCount--)| <b>@deprecated.</b> Please use the 'pageCount' property instead. Total page count. |
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
### getHasMorePages() {#getHasMorePages--}
```javascript
getHasMorePages() : boolean;
```
### setHasMorePages(boolean) {#setHasMorePages-boolean-}
```javascript
setHasMorePages(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getPageIndex() {#getPageIndex--}
```javascript
getPageIndex() : number;
```
### getPageCount() {#getPageCount--}
```javascript
getPageCount() : number;
```
