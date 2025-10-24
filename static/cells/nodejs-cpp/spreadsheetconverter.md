##SpreadsheetConverter
Converter for conversion between different spreadsheet file formats such as xls xlsx xlsb spreadsheet ml...
## SpreadsheetConverter class
Converter for conversion between different spreadsheet file formats, such as xls, xlsx, xlsb, spreadsheet ml...
```javascript
class SpreadsheetConverter;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [process(string, string)](#process-string-string-)| Converts given template file between spreadsheet file formats. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### process(string, string) {#process-string-string-}
Converts given template file between spreadsheet file formats.
```javascript
static process(templateFile: string, resultFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be converted |
| resultFile | string | The resultant file |
