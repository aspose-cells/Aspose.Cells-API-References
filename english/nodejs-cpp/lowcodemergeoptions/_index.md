---
title: LowCodeMergeOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for merging multiple template files into one.
type: docs
url: /nodejs-cpp/lowcodemergeoptions/
---

## LowCodeMergeOptions class

Options for merging multiple template files into one.

```javascript
class LowCodeMergeOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getSaveOptions()](#getSaveOptions--)| Save options for saving the split parts. |
| [setSaveOptions(LowCodeSaveOptions)](#setSaveOptions-lowcodesaveoptions-)| Save options for saving the split parts. |
| [getLoadOptionsProvider()](#getLoadOptionsProvider--)| Provider of save options for saving the split parts. |
| [setLoadOptionsProvider(AbstractLowCodeLoadOptionsProvider)](#setLoadOptionsProvider-abstractlowcodeloadoptionsprovider-)| Provider of save options for saving the split parts. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getSaveOptions() {#getSaveOptions--}

Save options for saving the split parts.

```javascript
getSaveOptions() : LowCodeSaveOptions;
```


**Returns**

[LowCodeSaveOptions](../lowcodesaveoptions/)

### setSaveOptions(LowCodeSaveOptions) {#setSaveOptions-lowcodesaveoptions-}

Save options for saving the split parts.

```javascript
setSaveOptions(value: LowCodeSaveOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../lowcodesaveoptions/) | The value to set. |

### getLoadOptionsProvider() {#getLoadOptionsProvider--}

Provider of save options for saving the split parts.

```javascript
getLoadOptionsProvider() : AbstractLowCodeLoadOptionsProvider;
```


**Returns**

[AbstractLowCodeLoadOptionsProvider](../abstractlowcodeloadoptionsprovider/)

**Remarks**

If this property is specified, [LoadOptions](../loadoptions/) takes no effect because the output of every split part will be specified by the provider.

### setLoadOptionsProvider(AbstractLowCodeLoadOptionsProvider) {#setLoadOptionsProvider-abstractlowcodeloadoptionsprovider-}

Provider of save options for saving the split parts.

```javascript
setLoadOptionsProvider(value: AbstractLowCodeLoadOptionsProvider) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractLowCodeLoadOptionsProvider](../abstractlowcodeloadoptionsprovider/) | The value to set. |

**Remarks**

If this property is specified, [LoadOptions](../loadoptions/) takes no effect because the output of every split part will be specified by the provider.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



