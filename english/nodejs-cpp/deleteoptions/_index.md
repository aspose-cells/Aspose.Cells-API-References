﻿---
title: DeleteOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the setting of deleting rowscolumns.
type: docs
url: /nodejs-cpp/deleteoptions/
---

## DeleteOptions class

Represents the setting of deleting rows/columns.

```javascript
class DeleteOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getUpdateReference()](#getUpdateReference--)| Indicates if update references in other worksheets. |
| [setUpdateReference(boolean)](#setUpdateReference-boolean-)| Indicates if update references in other worksheets. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--)| Gets/sets the monitor for tracking changes caused by the deletion. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor)](#setFormulaChangeMonitor-abstractformulachangemonitor-)| Gets/sets the monitor for tracking changes caused by the deletion. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getUpdateReference() {#getUpdateReference--}

Indicates if update references in other worksheets.

```javascript
getUpdateReference() : boolean;
```


### setUpdateReference(boolean) {#setUpdateReference-boolean-}

Indicates if update references in other worksheets.

```javascript
setUpdateReference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}

Gets/sets the monitor for tracking changes caused by the deletion.

```javascript
getFormulaChangeMonitor() : AbstractFormulaChangeMonitor;
```


**Returns**

[AbstractFormulaChangeMonitor](../abstractformulachangemonitor/)

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor) {#setFormulaChangeMonitor-abstractformulachangemonitor-}

Gets/sets the monitor for tracking changes caused by the deletion.

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



