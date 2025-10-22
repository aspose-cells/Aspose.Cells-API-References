##PdfConverter
Converter for converting template file to pdf.
## PdfConverter class
Converter for converting template file to pdf.
```javascript
class PdfConverter;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [process(string, string)](#process-string-string-)| Converts given template file to pdf. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### process(string, string) {#process-string-string-}
Converts given template file to pdf.
```javascript
static process(templateFile: string, resultFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be converted |
| resultFile | string | The resultant file, it must be pdf file. |
