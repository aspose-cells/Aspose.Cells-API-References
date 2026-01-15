---
title: CellValue
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the cell value and corresponding type.
type: docs
url: /javascript-cpp/cellvalue/
---

## CellValue class

Represents the cell value and corresponding type.

```javascript
class CellValue;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| CellValueType | Gets or sets the type of cell value. |
| [value](#value--)| VObject | Gets or sets the cell value. |


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
value : VObject;
```


**Remarks**

The value must be of the correct type of object corresponding to the [Type](../type/): <list type="table"> <listheader> <description>Type</description> <description>Value</description> </listheader> <item> <description>[CellValueType.IsNull](../cellvaluetype.isnull/)</description> <description>null, any other object will be ignored</description> </item> <item> <description>[CellValueType.IsNumeric](../cellvaluetype.isnumeric/)</description> <description>double</description> </item> <item> <description>[CellValueType.IsDateTime](../cellvaluetype.isdatetime/)</description> <description>DateTime</description> </item> <item> <description>[CellValueType.IsString](../cellvaluetype.isstring/)</description> <description>string</description> </item> <item> <description>[CellValueType.IsBool](../cellvaluetype.isbool/)</description> <description>bool</description> </item> <item> <description>[CellValueType.IsError](../cellvaluetype.iserror/)</description> <description>error string such as "#VALUE!", "#NAME?", ...</description> </item> </list


