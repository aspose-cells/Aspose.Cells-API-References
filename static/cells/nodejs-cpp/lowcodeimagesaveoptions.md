##LowCodeImageSaveOptions
Options for saving image in low code way.
## LowCodeImageSaveOptions class
Options for saving image in low code way.
```javascript
class LowCodeImageSaveOptions extends LowCodeSaveOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(LowCodeSaveOptions)](#constructor-lowcodesaveoptions-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [imageOptions](#imageOptions--)| ImageOrPrintOptions | The options for rendering images. |
| [saveOptionsProvider](#saveOptionsProvider--)| AbstractLowCodeSaveOptionsProvider | Provider of save options for saving generated images. |
| [outputFile](#outputFile--)| string | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [outputStream](#outputStream--)| Uint8Array | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |
## Methods
| Method | Description |
| --- | --- |
| [getImageOptions()](#getImageOptions--)| <b>@deprecated.</b> Please use the 'imageOptions' property instead. The options for rendering images. |
| [setImageOptions(ImageOrPrintOptions)](#setImageOptions-imageorprintoptions-)| <b>@deprecated.</b> Please use the 'imageOptions' property instead. The options for rendering images. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--)| <b>@deprecated.</b> Please use the 'saveOptionsProvider' property instead. Provider of save options for saving generated images. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider)](#setSaveOptionsProvider-abstractlowcodesaveoptionsprovider-)| <b>@deprecated.</b> Please use the 'saveOptionsProvider' property instead. Provider of save options for saving generated images. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getOutputFile()](#getOutputFile--)| <b>@deprecated.</b> Please use the 'outputFile' property instead. Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [setOutputFile(string)](#setOutputFile-string-)| <b>@deprecated.</b> Please use the 'outputFile' property instead. Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [getOutputStream()](#getOutputStream--)| <b>@deprecated.</b> Please use the 'outputStream' property instead. Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |
| [setOutputStream(Uint8Array)](#setOutputStream-uint8array-)| <b>@deprecated.</b> Please use the 'outputStream' property instead. Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |
| [getSaveFormat()](#getSaveFormat--)| Gets or sets the save format. |
| [setSaveFormat(SaveFormat)](#setSaveFormat-saveformat-)| Gets or sets the save format. |
### constructor(LowCodeSaveOptions) {#constructor-lowcodesaveoptions-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: LowCodeSaveOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | LowCodeSaveOptions | The parent object. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### imageOptions {#imageOptions--}
The options for rendering images.
```javascript
imageOptions : ImageOrPrintOptions;
```
**Remarks**
When one [ImageOrPrintOptions](../imageorprintoptions/) instance is specified, the [SaveFormat](../saveformat/) will be overwritten(if it had been specified before).
### saveOptionsProvider {#saveOptionsProvider--}
Provider of save options for saving generated images.
```javascript
saveOptionsProvider : AbstractLowCodeSaveOptionsProvider;
```
**Remarks**
The output([LowCodeSaveOptions.OutputFile](../lowcodesaveoptions.outputfile/) or [LowCodeSaveOptions.OutputStream](../lowcodesaveoptions.outputstream/)) specified by this instance will take no effect when this property is specified. Instead the output of every generated image will be specified by the provider.
### outputFile {#outputFile--}
Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored.
```javascript
outputFile : string;
```
### outputStream {#outputStream--}
Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored.
```javascript
outputStream : Uint8Array;
```
### getImageOptions() {#getImageOptions--}
```javascript
getImageOptions() : ImageOrPrintOptions;
```
**Returns**
[ImageOrPrintOptions](../imageorprintoptions/)
**Remarks**
When one [ImageOrPrintOptions](../imageorprintoptions/) instance is specified, the [SaveFormat](../saveformat/) will be overwritten(if it had been specified before).
### setImageOptions(ImageOrPrintOptions) {#setImageOptions-imageorprintoptions-}
```javascript
setImageOptions(value: ImageOrPrintOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../imageorprintoptions/) | The value to set. |
**Remarks**
When one [ImageOrPrintOptions](../imageorprintoptions/) instance is specified, the [SaveFormat](../saveformat/) will be overwritten(if it had been specified before).
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```javascript
getSaveOptionsProvider() : AbstractLowCodeSaveOptionsProvider;
```
**Returns**
[AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
**Remarks**
The output([LowCodeSaveOptions.OutputFile](../lowcodesaveoptions.outputfile/) or [LowCodeSaveOptions.OutputStream](../lowcodesaveoptions.outputstream/)) specified by this instance will take no effect when this property is specified. Instead the output of every generated image will be specified by the provider.
### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider) {#setSaveOptionsProvider-abstractlowcodesaveoptionsprovider-}
```javascript
setSaveOptionsProvider(value: AbstractLowCodeSaveOptionsProvider) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/) | The value to set. |
**Remarks**
The output([LowCodeSaveOptions.OutputFile](../lowcodesaveoptions.outputfile/) or [LowCodeSaveOptions.OutputStream](../lowcodesaveoptions.outputstream/)) specified by this instance will take no effect when this property is specified. Instead the output of every generated image will be specified by the provider.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getOutputFile() {#getOutputFile--}
```javascript
getOutputFile() : string;
```
### setOutputFile(string) {#setOutputFile-string-}
```javascript
setOutputFile(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getOutputStream() {#getOutputStream--}
```javascript
getOutputStream() : Uint8Array;
```
### setOutputStream(Uint8Array) {#setOutputStream-uint8array-}
```javascript
setOutputStream(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Uint8Array | The value to set. |
### getSaveFormat() {#getSaveFormat--}
Gets or sets the save format.
```javascript
getSaveFormat() : SaveFormat;
```
**Returns**
[SaveFormat](../saveformat/)
**Remarks**
If [ImageOptions](../imageoptions/) has been specified, setting this property will also change the [ImageOrPrintOptions.ImageType](../imageorprintoptions.imagetype/) value of it.
### setSaveFormat(SaveFormat) {#setSaveFormat-saveformat-}
Gets or sets the save format.
```javascript
setSaveFormat(value: SaveFormat) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SaveFormat](../saveformat/) | The value to set. |
**Remarks**
If [ImageOptions](../imageoptions/) has been specified, setting this property will also change the [ImageOrPrintOptions.ImageType](../imageorprintoptions.imagetype/) value of it.
