##ExternalLink
Represents an external link in a workbook.
## ExternalLink class
Represents an external link in a workbook.
```javascript
class ExternalLink;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
//Open a file with external links
var workbook = new Workbook("input/Externlink.xls");
//Get External Link
var externalLink = workbook.worksheets.externalLinks.get(0);
//Change External Link's Data Source
externalLink.dataSource = "input/Book1.xls";
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| ExternalLinkType | Readonly. Gets the type of external link. |
| [pathType](#pathType--)| string | Readonly. Get the path type of this external link |
| [originalDataSource](#originalDataSource--)| string | Represents stored data source of the external link. |
| [dataSource](#dataSource--)| string | Represents data source of the external link. |
| [isReferred](#isReferred--)| boolean | Readonly. Indicates whether this external link is referenced by others. |
| [isVisible](#isVisible--)| boolean | Readonly. Indicates whether this external link is visible in MS Excel. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the type of external link. |
| [getPathType()](#getPathType--)| <b>@deprecated.</b> Please use the 'pathType' property instead. Get the path type of this external link |
| [getOriginalDataSource()](#getOriginalDataSource--)| <b>@deprecated.</b> Please use the 'originalDataSource' property instead. Represents stored data source of the external link. |
| [setOriginalDataSource(string)](#setOriginalDataSource-string-)| <b>@deprecated.</b> Please use the 'originalDataSource' property instead. Represents stored data source of the external link. |
| [getDataSource()](#getDataSource--)| <b>@deprecated.</b> Please use the 'dataSource' property instead. Represents data source of the external link. |
| [setDataSource(string)](#setDataSource-string-)| <b>@deprecated.</b> Please use the 'dataSource' property instead. Represents data source of the external link. |
| [isReferred()](#isReferred--)| <b>@deprecated.</b> Please use the 'isReferred' property instead. Indicates whether this external link is referenced by others. |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Indicates whether this external link is visible in MS Excel. |
| [addExternalName(string, string)](#addExternalName-string-string-)| Adds an external name. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### type {#type--}
Readonly. Gets the type of external link.
```javascript
type : ExternalLinkType;
```
### pathType {#pathType--}
Readonly. Get the path type of this external link
```javascript
pathType : string;
```
### originalDataSource {#originalDataSource--}
Represents stored data source of the external link.
```javascript
originalDataSource : string;
```
### dataSource {#dataSource--}
Represents data source of the external link.
```javascript
dataSource : string;
```
### isReferred {#isReferred--}
Readonly. Indicates whether this external link is referenced by others.
```javascript
isReferred : boolean;
```
### isVisible {#isVisible--}
Readonly. Indicates whether this external link is visible in MS Excel.
```javascript
isVisible : boolean;
```
### getType() {#getType--}
```javascript
getType() : ExternalLinkType;
```
**Returns**
[ExternalLinkType](../externallinktype/)
### getPathType() {#getPathType--}
```javascript
getPathType() : string;
```
### getOriginalDataSource() {#getOriginalDataSource--}
```javascript
getOriginalDataSource() : string;
```
### setOriginalDataSource(string) {#setOriginalDataSource-string-}
```javascript
setOriginalDataSource(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getDataSource() {#getDataSource--}
```javascript
getDataSource() : string;
```
### setDataSource(string) {#setDataSource-string-}
```javascript
setDataSource(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isReferred() {#isReferred--}
```javascript
isReferred() : boolean;
```
### isVisible() {#isVisible--}
```javascript
isVisible() : boolean;
```
### addExternalName(string, string) {#addExternalName-string-string-}
Adds an external name.
```javascript
addExternalName(text: string, referTo: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text of the external name.         /// If the external name belongs to a worksheet, the text should be as Sheet1!Text. |
| referTo | string | The referTo of the external name. It must be a cell or the range. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
