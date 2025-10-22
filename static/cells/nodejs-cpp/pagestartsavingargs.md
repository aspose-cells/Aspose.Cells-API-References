##PageStartSavingArgs
Info for a page starts saving process.
## PageStartSavingArgs class
Info for a page starts saving process.
```javascript
class PageStartSavingArgs extends PageSavingArgs;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(PageSavingArgs)](#constructor-pagesavingargs-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isToOutput](#isToOutput--)| boolean | Gets or sets a value indicating whether the page should be output. The default value is true. |
| [pageIndex](#pageIndex--)| number | Readonly. Current page index, zero based. |
| [pageCount](#pageCount--)| number | Readonly. Total page count. |
## Methods
| Method | Description |
| --- | --- |
| [isToOutput()](#isToOutput--)| <b>@deprecated.</b> Please use the 'isToOutput' property instead. Gets or sets a value indicating whether the page should be output. The default value is true. |
| [setIsToOutput(boolean)](#setIsToOutput-boolean-)| <b>@deprecated.</b> Please use the 'isToOutput' property instead. Gets or sets a value indicating whether the page should be output. The default value is true. |
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
### isToOutput {#isToOutput--}
Gets or sets a value indicating whether the page should be output. The default value is true.
```javascript
isToOutput : boolean;
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
### isToOutput() {#isToOutput--}
```javascript
isToOutput() : boolean;
```
### setIsToOutput(boolean) {#setIsToOutput-boolean-}
```javascript
setIsToOutput(value: boolean) : void;
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
