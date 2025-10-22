##JsonConverter
Converter for conversion between json data structure and other spreadsheet file formats.
## JsonConverter class
Converter for conversion between json data structure and other spreadsheet file formats.
```javascript
class JsonConverter;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [process(string, string)](#process-string-string-)| Converts given template file between json and other formats. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### process(string, string) {#process-string-string-}
Converts given template file between json and other formats.
```javascript
static process(templateFile: string, resultFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be converted |
| resultFile | string | The resultant file |
