##ImageConverter
Converter for converting template file to images.
## ImageConverter class
Converter for converting template file to images.
```javascript
class ImageConverter;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [process(string, string)](#process-string-string-)| Converts template file to images. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### process(string, string) {#process-string-string-}
Converts template file to images.
```javascript
static process(templateFile: string, resultFile: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be converted to images. |
| resultFile | string | The resultant file(name pattern) for generated images. |
**Remarks**
The output files will be build from the specified result file by appending sequence number of the sheet and split part. For example, if the specified output file is Image.png, then the generated image files will be Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...
