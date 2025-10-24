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
