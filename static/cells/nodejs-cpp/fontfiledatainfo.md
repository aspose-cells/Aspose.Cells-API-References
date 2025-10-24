##FontFileDataInfo
Represents data infomation of font file data.
## FontFileDataInfo class
Represents data infomation of font file data.
```javascript
class FontFileDataInfo;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [data](#data--)| Uint8Array | Readonly. Gets binary data of font file. |
| [formatType](#formatType--)| FontFileFormatType | Readonly. Gets font format type of font file. |
## Methods
| Method | Description |
| --- | --- |
| [getData()](#getData--)| <b>@deprecated.</b> Please use the 'data' property instead. Gets binary data of font file. |
| [getFormatType()](#getFormatType--)| <b>@deprecated.</b> Please use the 'formatType' property instead. Gets font format type of font file. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### data {#data--}
Readonly. Gets binary data of font file.
```javascript
data : Uint8Array;
```
### formatType {#formatType--}
Readonly. Gets font format type of font file.
```javascript
formatType : FontFileFormatType;
```
### getData() {#getData--}
```javascript
getData() : Uint8Array;
```
### getFormatType() {#getFormatType--}
```javascript
getFormatType() : FontFileFormatType;
```
**Returns**
[FontFileFormatType](../fontfileformattype/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
