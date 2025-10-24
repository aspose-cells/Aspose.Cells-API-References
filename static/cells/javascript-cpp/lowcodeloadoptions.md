##LowCodeLoadOptions
Options for loading template file.
## LowCodeLoadOptions class
Options for loading template file.
```javascript
class LowCodeLoadOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [inputFile](#inputFile--)| string | Gets and sets the file(with path if needed) of the template. |
| [inputStream](#inputStream--)| Uint8Array | Gets and sets the Stream of the template. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### inputFile {#inputFile--}
Gets and sets the file(with path if needed) of the template.
```javascript
inputFile : string;
```
**Remarks**
When setting a non-null and non-empty path to this property, the previously set value for [InputStream](../inputstream/) will be ignored.
### inputStream {#inputStream--}
Gets and sets the Stream of the template.
```javascript
inputStream : Uint8Array;
```
**Remarks**
When setting a non-null Stream to this property, the previously set value for [InputFile](../inputfile/) will be ignored.
