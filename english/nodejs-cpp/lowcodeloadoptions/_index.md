---
title: LowCodeLoadOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for loading template file.
type: docs
url: /nodejs-cpp/lowcodeloadoptions/
---

## LowCodeLoadOptions class

Options for loading template file.

```javascript
class LowCodeLoadOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getInputFile()](#getInputFile--)| Gets and sets the file(with path if needed) of the template. |
| [setInputFile(string)](#setInputFile-string-)| Gets and sets the file(with path if needed) of the template. |
| [getInputStream()](#getInputStream--)| Gets and sets the Stream of the template. |
| [setInputStream(Uint8Array)](#setInputStream-uint8array-)| Gets and sets the Stream of the template. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getInputFile() {#getInputFile--}

Gets and sets the file(with path if needed) of the template.

```javascript
getInputFile() : string;
```


**Remarks**

When setting a non-null and non-empty path to this property, the previously set value for [InputStream](../inputstream/) will be ignored.

### setInputFile(string) {#setInputFile-string-}

Gets and sets the file(with path if needed) of the template.

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

Gets and sets the Stream of the template.

```javascript
getInputStream() : Uint8Array;
```


**Remarks**

When setting a non-null Stream to this property, the previously set value for [InputFile](../inputfile/) will be ignored.

### setInputStream(Uint8Array) {#setInputStream-uint8array-}

Gets and sets the Stream of the template.

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



