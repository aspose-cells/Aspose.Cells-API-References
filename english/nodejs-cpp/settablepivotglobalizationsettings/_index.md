﻿---
title: SettablePivotGlobalizationSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Implementation of PivotGlobalizationSettings that supports user to setchange predefined texts.
type: docs
url: /nodejs-cpp/settablepivotglobalizationsettings/
---

## SettablePivotGlobalizationSettings class

Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.

```javascript
class SettablePivotGlobalizationSettings;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getTextOfTotal()](#getTextOfTotal--)| Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area. |
| [setTextOfTotal(string)](#setTextOfTotal-string-)| Sets the text of "Total" label in the PivotTable. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--)| Gets the text of "Grand Total" label in the PivotTable. |
| [setTextOfGrandTotal(string)](#setTextOfGrandTotal-string-)| Sets the text of "Grand Total" label in the PivotTable. |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--)| Gets the text of "(Multiple Items)" label in the PivotTable. |
| [setTextOfMultipleItems(string)](#setTextOfMultipleItems-string-)| Sets the text of "(Multiple Items)" label in the PivotTable. |
| [getTextOfAll()](#getTextOfAll--)| Gets the text of "(All)" label in the PivotTable. |
| [setTextOfAll(string)](#setTextOfAll-string-)| Sets the text of "(All)" label in the PivotTable. |
| [getTextOfProtectedName(string)](#getTextOfProtectedName-string-)| Gets the text for specified protected name. |
| [setTextOfProtectedName(string, string)](#setTextOfProtectedName-string-string-)| Sets the text for specific protected name. |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--)| Gets the text of "Column Labels" label in the PivotTable. |
| [setTextOfColumnLabels(string)](#setTextOfColumnLabels-string-)| Gets the text of "Column Labels" label in the PivotTable. |
| [getTextOfRowLabels()](#getTextOfRowLabels--)| Gets the text of "Row Labels" label in the PivotTable. |
| [setTextOfRowLabels(string)](#setTextOfRowLabels-string-)| Sets the text of "Row Labels" label in the PivotTable. |
| [getTextOfEmptyData()](#getTextOfEmptyData--)| Gets the text of "(blank)" label in the PivotTable. |
| [setTextOfEmptyData(string)](#setTextOfEmptyData-string-)| Sets the text of "(blank)" label in the PivotTable. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--)| Gets the the text of the value area field header in the PivotTable. |
| [setTextOfDataFieldHeader(string)](#setTextOfDataFieldHeader-string-)| Sets the the text of the value area field header in the PivotTable. |
| [getTextOfSubTotal(PivotFieldSubtotalType)](#getTextOfSubTotal-pivotfieldsubtotaltype-)| Gets the text of [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) type in the PivotTable. |
| [setTextOfSubTotal(PivotFieldSubtotalType, string)](#setTextOfSubTotal-pivotfieldsubtotaltype-string-)| Sets the text of [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) type in the PivotTable. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getTextOfTotal() {#getTextOfTotal--}

Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

```javascript
getTextOfTotal() : string;
```


**Returns**

The text of "Total" label

### setTextOfTotal(string) {#setTextOfTotal-string-}

Sets the text of "Total" label in the PivotTable.

```javascript
setTextOfTotal(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | custom text |

### getTextOfGrandTotal() {#getTextOfGrandTotal--}

Gets the text of "Grand Total" label in the PivotTable.

```javascript
getTextOfGrandTotal() : string;
```


**Returns**

The text of "Grand Total" label

### setTextOfGrandTotal(string) {#setTextOfGrandTotal-string-}

Sets the text of "Grand Total" label in the PivotTable.

```javascript
setTextOfGrandTotal(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | custom text |

### getTextOfMultipleItems() {#getTextOfMultipleItems--}

Gets the text of "(Multiple Items)" label in the PivotTable.

```javascript
getTextOfMultipleItems() : string;
```


**Returns**

The text of "(Multiple Items)" label

### setTextOfMultipleItems(string) {#setTextOfMultipleItems-string-}

Sets the text of "(Multiple Items)" label in the PivotTable.

```javascript
setTextOfMultipleItems(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | custom text |

### getTextOfAll() {#getTextOfAll--}

Gets the text of "(All)" label in the PivotTable.

```javascript
getTextOfAll() : string;
```


**Returns**

The text of "(All)" label

### setTextOfAll(string) {#setTextOfAll-string-}

Sets the text of "(All)" label in the PivotTable.

```javascript
setTextOfAll(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | custom text |

### getTextOfProtectedName(string) {#getTextOfProtectedName-string-}

Gets the text for specified protected name.

```javascript
getTextOfProtectedName(protectedName: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | string | The protected name in PivotTable. |

**Returns**

The local prorected names of PivotTable.

**Remarks**

In Ms Excel, some names are not allowed to be used as the name of PivotFields in PivotTable. They are different in different region, user may specify them explicitly according to the used region.

### setTextOfProtectedName(string, string) {#setTextOfProtectedName-string-string-}

Sets the text for specific protected name.

```javascript
setTextOfProtectedName(protectedName: string, text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | string | The protected name in PivotTable. |
| text | string | The local prorected names of PivotTable. |

### getTextOfColumnLabels() {#getTextOfColumnLabels--}

Gets the text of "Column Labels" label in the PivotTable.

```javascript
getTextOfColumnLabels() : string;
```


**Returns**

The text of column labels

### setTextOfColumnLabels(string) {#setTextOfColumnLabels-string-}

Gets the text of "Column Labels" label in the PivotTable.

```javascript
setTextOfColumnLabels(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text of column labels |

### getTextOfRowLabels() {#getTextOfRowLabels--}

Gets the text of "Row Labels" label in the PivotTable.

```javascript
getTextOfRowLabels() : string;
```


**Returns**

The text of row labels

### setTextOfRowLabels(string) {#setTextOfRowLabels-string-}

Sets the text of "Row Labels" label in the PivotTable.

```javascript
setTextOfRowLabels(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text of row labels |

### getTextOfEmptyData() {#getTextOfEmptyData--}

Gets the text of "(blank)" label in the PivotTable.

```javascript
getTextOfEmptyData() : string;
```


**Returns**

The text of empty data

### setTextOfEmptyData(string) {#setTextOfEmptyData-string-}

Sets the text of "(blank)" label in the PivotTable.

```javascript
setTextOfEmptyData(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text of empty data |

### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}

Gets the the text of the value area field header in the PivotTable.

```javascript
getTextOfDataFieldHeader() : string;
```


**Returns**

The text of data field header name

### setTextOfDataFieldHeader(string) {#setTextOfDataFieldHeader-string-}

Sets the the text of the value area field header in the PivotTable.

```javascript
setTextOfDataFieldHeader(text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text of data field header name |

### getTextOfSubTotal(PivotFieldSubtotalType) {#getTextOfSubTotal-pivotfieldsubtotaltype-}

Gets the text of [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) type in the PivotTable.

```javascript
getTextOfSubTotal(subTotalType: PivotFieldSubtotalType) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) |

**Returns**

The text of given type

### setTextOfSubTotal(PivotFieldSubtotalType, string) {#setTextOfSubTotal-pivotfieldsubtotaltype-string-}

Sets the text of [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) type in the PivotTable.

```javascript
setTextOfSubTotal(subTotalType: PivotFieldSubtotalType, text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) |
| text | string | The text of given type |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



