---
title: CellValue
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the cell value and corresponding type.
type: docs
url: /nodejs-cpp/cellvalue/
---

## CellValue class

Represents the cell value and corresponding type.

```javascript
class CellValue;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| CellValueType | Gets or sets the type of cell value. |
| [value](#value--)| Object | Gets or sets the cell value. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets or sets the type of cell value. |
| [setType(CellValueType)](#setType-cellvaluetype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets or sets the type of cell value. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets or sets the cell value. |
| [setValue(Object)](#setValue-object-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets or sets the cell value. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### type {#type--}

Gets or sets the type of cell value.

```javascript
type : CellValueType;
```


### value {#value--}

Gets or sets the cell value.

```javascript
value : Object;
```


**Remarks**

The value must be of the correct type of object corresponding to the [Type](../type/): <list type="table"> <listheader> <description>Type</description> <description>Value</description> </listheader> <item> <description>[CellValueType.IsNull](../cellvaluetype.isnull/)</description> <description>null, any other object will be ignored</description> </item> <item> <description>[CellValueType.IsNumeric](../cellvaluetype.isnumeric/)</description> <description>double</description> </item> <item> <description>[CellValueType.IsDateTime](../cellvaluetype.isdatetime/)</description> <description>DateTime</description> </item> <item> <description>[CellValueType.IsString](../cellvaluetype.isstring/)</description> <description>string</description> </item> <item> <description>[CellValueType.IsBool](../cellvaluetype.isbool/)</description> <description>bool</description> </item> <item> <description>[CellValueType.IsError](../cellvaluetype.iserror/)</description> <description>error string such as "#VALUE!", "#NAME?", ...</description> </item> </list

### getType() {#getType--}

<b>@deprecated.</b> Please use the 'type' property instead. Gets or sets the type of cell value.

```javascript
getType() : CellValueType;
```


**Returns**

[CellValueType](../cellvaluetype/)

### setType(CellValueType) {#setType-cellvaluetype-}

<b>@deprecated.</b> Please use the 'type' property instead. Gets or sets the type of cell value.

```javascript
setType(value: CellValueType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellValueType](../cellvaluetype/) | The value to set. |

### getValue() {#getValue--}

<b>@deprecated.</b> Please use the 'value' property instead. Gets or sets the cell value.

```javascript
getValue() : Object;
```


**Remarks**

The value must be of the correct type of object corresponding to the [Type](../type/): <list type="table"> <listheader> <description>Type</description> <description>Value</description> </listheader> <item> <description>[CellValueType.IsNull](../cellvaluetype.isnull/)</description> <description>null, any other object will be ignored</description> </item> <item> <description>[CellValueType.IsNumeric](../cellvaluetype.isnumeric/)</description> <description>double</description> </item> <item> <description>[CellValueType.IsDateTime](../cellvaluetype.isdatetime/)</description> <description>DateTime</description> </item> <item> <description>[CellValueType.IsString](../cellvaluetype.isstring/)</description> <description>string</description> </item> <item> <description>[CellValueType.IsBool](../cellvaluetype.isbool/)</description> <description>bool</description> </item> <item> <description>[CellValueType.IsError](../cellvaluetype.iserror/)</description> <description>error string such as "#VALUE!", "#NAME?", ...</description> </item> </list

### setValue(Object) {#setValue-object-}

<b>@deprecated.</b> Please use the 'value' property instead. Gets or sets the cell value.

```javascript
setValue(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

**Remarks**

The value must be of the correct type of object corresponding to the [Type](../type/): <list type="table"> <listheader> <description>Type</description> <description>Value</description> </listheader> <item> <description>[CellValueType.IsNull](../cellvaluetype.isnull/)</description> <description>null, any other object will be ignored</description> </item> <item> <description>[CellValueType.IsNumeric](../cellvaluetype.isnumeric/)</description> <description>double</description> </item> <item> <description>[CellValueType.IsDateTime](../cellvaluetype.isdatetime/)</description> <description>DateTime</description> </item> <item> <description>[CellValueType.IsString](../cellvaluetype.isstring/)</description> <description>string</description> </item> <item> <description>[CellValueType.IsBool](../cellvaluetype.isbool/)</description> <description>bool</description> </item> <item> <description>[CellValueType.IsError](../cellvaluetype.iserror/)</description> <description>error string such as "#VALUE!", "#NAME?", ...</description> </item> </list

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



