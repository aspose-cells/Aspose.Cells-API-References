##SpreadsheetMerger
Merges multiple template files into one.
## SpreadsheetMerger class
Merges multiple template files into one.
```javascript
class SpreadsheetMerger;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [process(string[], string)](#process-stringarray-string-)| Merge given template files. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### process(string[], string) {#process-stringarray-string-}
Merge given template files.
```javascript
static process(templateFiles: string[], resultFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFiles | string[] | The template files to be merged |
| resultFile | string | The resultant file |
