##RevisionLog
Represents the revision log.
## RevisionLog class
Represents the revision log.
```javascript
class RevisionLog;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [metadataTable](#metadataTable--)| RevisionHeader | Readonly. Gets table that contains metadata about a list of specific changes that have taken place for this workbook. |
| [revisions](#revisions--)| RevisionCollection | Readonly. Gets all revisions in this log. |
## Methods
| Method | Description |
| --- | --- |
| [getMetadataTable()](#getMetadataTable--)| <b>@deprecated.</b> Please use the 'metadataTable' property instead. Gets table that contains metadata about a list of specific changes that have taken place for this workbook. |
| [getRevisions()](#getRevisions--)| <b>@deprecated.</b> Please use the 'revisions' property instead. Gets all revisions in this log. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### metadataTable {#metadataTable--}
Readonly. Gets table that contains metadata about a list of specific changes that have taken place for this workbook.
```javascript
metadataTable : RevisionHeader;
```
### revisions {#revisions--}
Readonly. Gets all revisions in this log.
```javascript
revisions : RevisionCollection;
```
### getMetadataTable() {#getMetadataTable--}
```javascript
getMetadataTable() : RevisionHeader;
```
**Returns**
[RevisionHeader](../revisionheader/)
### getRevisions() {#getRevisions--}
```javascript
getRevisions() : RevisionCollection;
```
**Returns**
[RevisionCollection](../revisioncollection/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
