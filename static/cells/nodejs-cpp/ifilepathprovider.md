##IFilePathProvider
Represents the exported file path provider.
## IFilePathProvider interface
Represents the exported file path provider.
## Methods
| Method | Description |
| --- | --- |
| [getFullName(string)](#getFullName-string-)| Gets the full path of the file by Worksheet name when exporting Worksheet to html separately. So the references among the Worksheets can be exported correctly. |
### getFullName(string) {#getFullName-string-}
Gets the full path of the file by Worksheet name when exporting Worksheet to html separately. So the references among the Worksheets can be exported correctly.
```javascript
getFullName(sheetName: string) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | string | Worksheet name |
**Returns**
the full path of the file
