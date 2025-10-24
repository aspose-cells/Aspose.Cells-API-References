##PageStartSavingArgs
Info for a page starts saving process.
## PageStartSavingArgs class
Info for a page starts saving process.
```javascript
class PageStartSavingArgs extends PageSavingArgs;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(PageSavingArgs)](#constructor-pagesavingargs-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isToOutput](#isToOutput--)| boolean | Gets or sets a value indicating whether the page should be output. The default value is true. |
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
