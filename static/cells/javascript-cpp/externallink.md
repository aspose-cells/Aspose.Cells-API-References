##ExternalLink
Represents an external link in a workbook.
## ExternalLink class
Represents an external link in a workbook.
```javascript
class ExternalLink;
```
### Example
```javascript
const { Workbook } = AsposeCells;
//Open a file with external links
var workbook = new Workbook(data);
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
| [addExternalName(string, string)](#addExternalName-string-string-)| Adds an external name. |
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
