﻿---
title: LowCodeHtmlSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for saving html in low code way.
type: docs
url: /nodejs-cpp/lowcodehtmlsaveoptions/
---

## LowCodeHtmlSaveOptions class

Options for saving html in low code way.

```javascript
class LowCodeHtmlSaveOptions extends LowCodeSaveOptions;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor(LowCodeSaveOptions)](#constructor-lowcodesaveoptions-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [saveFormat](#saveFormat--)| SaveFormat | Gets and sets the format of spreadsheet. |
| [htmlOptions](#htmlOptions--)| HtmlSaveOptions | The general options for saving html. |
| [outputFile](#outputFile--)| string | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [outputStream](#outputStream--)| Uint8Array | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |

## Methods

| Method | Description |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--)| <b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets and sets the format of spreadsheet. |
| [setSaveFormat(SaveFormat)](#setSaveFormat-saveformat-)| <b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets and sets the format of spreadsheet. |
| [getHtmlOptions()](#getHtmlOptions--)| <b>@deprecated.</b> Please use the 'htmlOptions' property instead. The general options for saving html. |
| [setHtmlOptions(HtmlSaveOptions)](#setHtmlOptions-htmlsaveoptions-)| <b>@deprecated.</b> Please use the 'htmlOptions' property instead. The general options for saving html. |
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

Gets and sets the format of spreadsheet.

```javascript
saveFormat : SaveFormat;
```


**Remarks**

When changing this property, the save format specified by [HtmlOptions](../htmloptions/) will be ignored(if it had been specified before).

### htmlOptions {#htmlOptions--}

The general options for saving html.

```javascript
htmlOptions : HtmlSaveOptions;
```


**Remarks**

When one [HtmlSaveOptions](../htmlsaveoptions/) instance is specified, the [SaveFormat](../saveformat/) will be overwritten(if it had been specified before).

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

<b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets and sets the format of spreadsheet.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

**Remarks**

When changing this property, the save format specified by [HtmlOptions](../htmloptions/) will be ignored(if it had been specified before).

### setSaveFormat(SaveFormat) {#setSaveFormat-saveformat-}

<b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets and sets the format of spreadsheet.

```javascript
setSaveFormat(value: SaveFormat) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SaveFormat](../saveformat/) | The value to set. |

**Remarks**

When changing this property, the save format specified by [HtmlOptions](../htmloptions/) will be ignored(if it had been specified before).

### getHtmlOptions() {#getHtmlOptions--}

<b>@deprecated.</b> Please use the 'htmlOptions' property instead. The general options for saving html.

```javascript
getHtmlOptions() : HtmlSaveOptions;
```


**Returns**

[HtmlSaveOptions](../htmlsaveoptions/)

**Remarks**

When one [HtmlSaveOptions](../htmlsaveoptions/) instance is specified, the [SaveFormat](../saveformat/) will be overwritten(if it had been specified before).

### setHtmlOptions(HtmlSaveOptions) {#setHtmlOptions-htmlsaveoptions-}

<b>@deprecated.</b> Please use the 'htmlOptions' property instead. The general options for saving html.

```javascript
setHtmlOptions(value: HtmlSaveOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlSaveOptions](../htmlsaveoptions/) | The value to set. |

**Remarks**

When one [HtmlSaveOptions](../htmlsaveoptions/) instance is specified, the [SaveFormat](../saveformat/) will be overwritten(if it had been specified before).

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


