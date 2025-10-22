##LowCodeLoadOptions
Options for loading template file.
## LowCodeLoadOptions class
Options for loading template file.
```javascript
class LowCodeLoadOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [inputFile](#inputFile--)| string | Gets and sets the file(with path if needed) of the template. |
| [inputStream](#inputStream--)| Uint8Array | Gets and sets the Stream of the template. |
## Methods
| Method | Description |
| --- | --- |
| [getInputFile()](#getInputFile--)| <b>@deprecated.</b> Please use the 'inputFile' property instead. Gets and sets the file(with path if needed) of the template. |
| [setInputFile(string)](#setInputFile-string-)| <b>@deprecated.</b> Please use the 'inputFile' property instead. Gets and sets the file(with path if needed) of the template. |
| [getInputStream()](#getInputStream--)| <b>@deprecated.</b> Please use the 'inputStream' property instead. Gets and sets the Stream of the template. |
| [setInputStream(Uint8Array)](#setInputStream-uint8array-)| <b>@deprecated.</b> Please use the 'inputStream' property instead. Gets and sets the Stream of the template. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getInputFile() {#getInputFile--}
```javascript
getInputFile() : string;
```
**Remarks**
When setting a non-null and non-empty path to this property, the previously set value for [InputStream](../inputstream/) will be ignored.
### setInputFile(string) {#setInputFile-string-}
```javascript
setInputFile(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
When setting a non-null and non-empty path to this property, the previously set value for [InputStream](../inputstream/) will be ignored.
### getInputStream() {#getInputStream--}
```javascript
getInputStream() : Uint8Array;
```
**Remarks**
When setting a non-null Stream to this property, the previously set value for [InputFile](../inputfile/) will be ignored.
### setInputStream(Uint8Array) {#setInputStream-uint8array-}
```javascript
setInputStream(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Uint8Array | The value to set. |
**Remarks**
When setting a non-null Stream to this property, the previously set value for [InputFile](../inputfile/) will be ignored.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
