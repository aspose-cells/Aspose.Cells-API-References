---
title: LowCodePdfSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for saving pdf in low code way.
type: docs
url: /nodejs-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

Options for saving pdf in low code way.

```javascript
class LowCodePdfSaveOptions extends LowCodeSaveOptions;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor(LowCodeSaveOptions)](#constructor-lowcodesaveoptions-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [saveFormat](#saveFormat--)| SaveFormat | The save format for the output. For converting to pdf, it can only be [SaveFormat.Pdf](../saveformat.pdf/). |
| [pdfOptions](#pdfOptions--)| PdfSaveOptions | The options for saving Pdf file. |
| [outputFile](#outputFile--)| string | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [outputStream](#outputStream--)| Uint8Array | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |

## Methods

| Method | Description |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--)| <b>@deprecated.</b> Please use the 'saveFormat' property instead. The save format for the output. For converting to pdf, it can only be [SaveFormat.Pdf](../saveformat.pdf/). |
| [setSaveFormat(SaveFormat)](#setSaveFormat-saveformat-)| <b>@deprecated.</b> Please use the 'saveFormat' property instead. The save format for the output. For converting to pdf, it can only be [SaveFormat.Pdf](../saveformat.pdf/). |
| [getPdfOptions()](#getPdfOptions--)| <b>@deprecated.</b> Please use the 'pdfOptions' property instead. The options for saving Pdf file. |
| [setPdfOptions(PdfSaveOptions)](#setPdfOptions-pdfsaveoptions-)| <b>@deprecated.</b> Please use the 'pdfOptions' property instead. The options for saving Pdf file. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getOutputFile()](#getOutputFile--)| <b>@deprecated.</b> Please use the 'outputFile' property instead. Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [setOutputFile(string)](#setOutputFile-string-)| <b>@deprecated.</b> Please use the 'outputFile' property instead. Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [getOutputStream()](#getOutputStream--)| <b>@deprecated.</b> Please use the 'outputStream' property instead. Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |
| [setOutputStream(Uint8Array)](#setOutputStream-uint8array-)| <b>@deprecated.</b> Please use the 'outputStream' property instead. Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |


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


### saveFormat {#saveFormat--}

The save format for the output. For converting to pdf, it can only be [SaveFormat.Pdf](../saveformat.pdf/).

```javascript
saveFormat : SaveFormat;
```


### pdfOptions {#pdfOptions--}

The options for saving Pdf file.

```javascript
pdfOptions : PdfSaveOptions;
```


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


### getSaveFormat() {#getSaveFormat--}

<b>@deprecated.</b> Please use the 'saveFormat' property instead. The save format for the output. For converting to pdf, it can only be [SaveFormat.Pdf](../saveformat.pdf/).

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

### setSaveFormat(SaveFormat) {#setSaveFormat-saveformat-}

<b>@deprecated.</b> Please use the 'saveFormat' property instead. The save format for the output. For converting to pdf, it can only be [SaveFormat.Pdf](../saveformat.pdf/).

```javascript
setSaveFormat(value: SaveFormat) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SaveFormat](../saveformat/) | The value to set. |

### getPdfOptions() {#getPdfOptions--}

<b>@deprecated.</b> Please use the 'pdfOptions' property instead. The options for saving Pdf file.

```javascript
getPdfOptions() : PdfSaveOptions;
```


**Returns**

[PdfSaveOptions](../pdfsaveoptions/)

### setPdfOptions(PdfSaveOptions) {#setPdfOptions-pdfsaveoptions-}

<b>@deprecated.</b> Please use the 'pdfOptions' property instead. The options for saving Pdf file.

```javascript
setPdfOptions(value: PdfSaveOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfSaveOptions](../pdfsaveoptions/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getOutputFile() {#getOutputFile--}

<b>@deprecated.</b> Please use the 'outputFile' property instead. Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored.

```javascript
getOutputFile() : string;
```


### setOutputFile(string) {#setOutputFile-string-}

<b>@deprecated.</b> Please use the 'outputFile' property instead. Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored.

```javascript
setOutputFile(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getOutputStream() {#getOutputStream--}

<b>@deprecated.</b> Please use the 'outputStream' property instead. Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored.

```javascript
getOutputStream() : Uint8Array;
```


### setOutputStream(Uint8Array) {#setOutputStream-uint8array-}

<b>@deprecated.</b> Please use the 'outputStream' property instead. Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored.

```javascript
setOutputStream(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Uint8Array | The value to set. |


