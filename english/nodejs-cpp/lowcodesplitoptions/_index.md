---
title: LowCodeSplitOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for splitting spreadsheet.
type: docs
url: /nodejs-cpp/lowcodesplitoptions/
---

## LowCodeSplitOptions class

Options for splitting spreadsheet.

```javascript
class LowCodeSplitOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getLoadOptions()](#getLoadOptions--)| Load options for loading the spreadsheet that will be split. |
| [setLoadOptions(LowCodeLoadOptions)](#setLoadOptions-lowcodeloadoptions-)| Load options for loading the spreadsheet that will be split. |
| [getSaveOptions()](#getSaveOptions--)| Save options for saving the split parts. |
| [setSaveOptions(LowCodeSaveOptions)](#setSaveOptions-lowcodesaveoptions-)| Save options for saving the split parts. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--)| Provider of save options for saving the split parts. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider)](#setSaveOptionsProvider-abstractlowcodesaveoptionsprovider-)| Provider of save options for saving the split parts. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getLoadOptions() {#getLoadOptions--}

Load options for loading the spreadsheet that will be split.

```javascript
getLoadOptions() : LowCodeLoadOptions;
```


**Returns**

[LowCodeLoadOptions](../lowcodeloadoptions/)

### setLoadOptions(LowCodeLoadOptions) {#setLoadOptions-lowcodeloadoptions-}

Load options for loading the spreadsheet that will be split.

```javascript
setLoadOptions(value: LowCodeLoadOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LowCodeLoadOptions](../lowcodeloadoptions/) | The value to set. |

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

### getSaveOptionsProvider() {#getSaveOptionsProvider--}

Provider of save options for saving the split parts.

```javascript
getSaveOptionsProvider() : AbstractLowCodeSaveOptionsProvider;
```


**Returns**

[AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)

**Remarks**

If this property is specified, [SaveOptions](../saveoptions/) takes no effect because the output of every split part will be specified by the provider.

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider) {#setSaveOptionsProvider-abstractlowcodesaveoptionsprovider-}

Provider of save options for saving the split parts.

```javascript
setSaveOptionsProvider(value: AbstractLowCodeSaveOptionsProvider) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/) | The value to set. |

**Remarks**

If this property is specified, [SaveOptions](../saveoptions/) takes no effect because the output of every split part will be specified by the provider.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



