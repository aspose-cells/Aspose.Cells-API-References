---
title: LowCodeSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for saving generated results in low code way.
type: docs
url: /nodejs-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

Options for saving generated results in low code way.

```javascript
class LowCodeSaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getOutputFile()](#getOutputFile--)| Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [setOutputFile(string)](#setOutputFile-string-)| Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored. |
| [getOutputStream()](#getOutputStream--)| Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |
| [setOutputStream(Uint8Array)](#setOutputStream-uint8array-)| Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSaveFormat()](#getSaveFormat--)| Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused. |
| [setSaveFormat(SaveFormat)](#setSaveFormat-saveformat-)| Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getOutputFile() {#getOutputFile--}

Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored.

```javascript
getOutputFile() : string;
```


### setOutputFile(string) {#setOutputFile-string-}

Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [OutputStream](../outputstream/) will be ignored.

```javascript
setOutputFile(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getOutputStream() {#getOutputStream--}

Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored.

```javascript
getOutputStream() : Uint8Array;
```


### setOutputStream(Uint8Array) {#setOutputStream-uint8array-}

Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [OutputFile](../outputfile/) will be ignored.

```javascript
setOutputStream(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Uint8Array | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getSaveFormat() {#getSaveFormat--}

Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

### setSaveFormat(SaveFormat) {#setSaveFormat-saveformat-}

Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused.

```javascript
setSaveFormat(value: SaveFormat) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SaveFormat](../saveformat/) | The value to set. |


