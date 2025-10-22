##TextConverter
Converter for conversion between text based formatscsv tsv dif... and other spreadsheet file formats.
## TextConverter class
Converter for conversion between text based formats(csv, tsv, dif...) and other spreadsheet file formats.
```javascript
class TextConverter;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [process(string, string)](#process-string-string-)| Converts given template file between text based files and other formats. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### process(string, string) {#process-string-string-}
Converts given template file between text based files and other formats.
```javascript
static process(templateFile: string, resultFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be converted |
| resultFile | string | The resultant file |
