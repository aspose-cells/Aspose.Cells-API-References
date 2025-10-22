##HtmlConverter
Converter for conversion between html fileshtml or mht and other spreadsheet file formats.
## HtmlConverter class
Converter for conversion between html files(html or mht) and other spreadsheet file formats.
```javascript
class HtmlConverter;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [process(string, string)](#process-string-string-)| Converts given template file between html and other formats. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### process(string, string) {#process-string-string-}
Converts given template file between html and other formats.
```javascript
static process(templateFile: string, resultFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be converted |
| resultFile | string | The resultant file |
