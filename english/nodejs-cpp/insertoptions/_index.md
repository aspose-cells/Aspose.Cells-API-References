---
title: InsertOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of inserting.
type: docs
url: /nodejs-cpp/insertoptions/
---

## InsertOptions class

Represents the options of inserting.

```javascript
class InsertOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getCopyFormatType()](#getCopyFormatType--)|  |
| [setCopyFormatType(CopyFormatType)](#setCopyFormatType-copyformattype-)|  |
| [getUpdateReference()](#getUpdateReference--)| Indicates if references in other worksheets will be updated. |
| [setUpdateReference(boolean)](#setUpdateReference-boolean-)| Indicates if references in other worksheets will be updated. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--)| Gets/sets the monitor for tracking changes caused by the insertion. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor)](#setFormulaChangeMonitor-abstractformulachangemonitor-)| Gets/sets the monitor for tracking changes caused by the insertion. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getCopyFormatType() {#getCopyFormatType--}



```javascript
getCopyFormatType() : CopyFormatType;
```


**Returns**

[CopyFormatType](../copyformattype/)

### setCopyFormatType(CopyFormatType) {#setCopyFormatType-copyformattype-}



```javascript
setCopyFormatType(value: CopyFormatType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CopyFormatType](../copyformattype/) | The value to set. |

### getUpdateReference() {#getUpdateReference--}

Indicates if references in other worksheets will be updated.

```javascript
getUpdateReference() : boolean;
```


### setUpdateReference(boolean) {#setUpdateReference-boolean-}

Indicates if references in other worksheets will be updated.

```javascript
setUpdateReference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}

Gets/sets the monitor for tracking changes caused by the insertion.

```javascript
getFormulaChangeMonitor() : AbstractFormulaChangeMonitor;
```


**Returns**

[AbstractFormulaChangeMonitor](../abstractformulachangemonitor/)

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor) {#setFormulaChangeMonitor-abstractformulachangemonitor-}

Gets/sets the monitor for tracking changes caused by the insertion.

```javascript
setFormulaChangeMonitor(value: AbstractFormulaChangeMonitor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../abstractformulachangemonitor/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



