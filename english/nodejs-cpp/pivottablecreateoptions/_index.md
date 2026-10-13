---
title: PivotTableCreateOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for creating a new PivotTable.
type: docs
url: /nodejs-cpp/pivottablecreateoptions/
---

## PivotTableCreateOptions class

Options for creating a new PivotTable.

```javascript
class PivotTableCreateOptions;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [tableName](#tableName--)| string | Gets or sets the name of the new PivotTable report. |
| [useSameSource](#useSameSource--)| boolean | Gets or sets a value indicating whether to share the same data source with existing pivot tables. Default value is true. |
| [isXlsClassic](#isXlsClassic--)| boolean | Gets or sets a value indicating whether to create classic Excel 97-2003 style PivotTable. |

## Methods

| Method | Description |
| --- | --- |
| [getTableName()](#getTableName--)| <b>@deprecated.</b> Please use the 'tableName' property instead. Gets or sets the name of the new PivotTable report. |
| [setTableName(string)](#setTableName-string-)| <b>@deprecated.</b> Please use the 'tableName' property instead. Gets or sets the name of the new PivotTable report. |
| [getUseSameSource()](#getUseSameSource--)| <b>@deprecated.</b> Please use the 'useSameSource' property instead. Gets or sets a value indicating whether to share the same data source with existing pivot tables. Default value is true. |
| [setUseSameSource(boolean)](#setUseSameSource-boolean-)| <b>@deprecated.</b> Please use the 'useSameSource' property instead. Gets or sets a value indicating whether to share the same data source with existing pivot tables. Default value is true. |
| [isXlsClassic()](#isXlsClassic--)| <b>@deprecated.</b> Please use the 'isXlsClassic' property instead. Gets or sets a value indicating whether to create classic Excel 97-2003 style PivotTable. |
| [setIsXlsClassic(boolean)](#setIsXlsClassic-boolean-)| <b>@deprecated.</b> Please use the 'isXlsClassic' property instead. Gets or sets a value indicating whether to create classic Excel 97-2003 style PivotTable. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### tableName {#tableName--}

Gets or sets the name of the new PivotTable report.

```javascript
tableName : string;
```


**Remarks**

If not set , an automatic name will be set.

### useSameSource {#useSameSource--}

Gets or sets a value indicating whether to share the same data source with existing pivot tables. Default value is true.

```javascript
useSameSource : boolean;
```


**Remarks**

When set to true, multiple pivot tables can reuse one pivot cache to reduce memory consumption.

### isXlsClassic {#isXlsClassic--}

Gets or sets a value indicating whether to create classic Excel 97-2003 style PivotTable.

```javascript
isXlsClassic : boolean;
```


**Remarks**

Classic PivotTable uses legacy layout and formatting from Excel 97-2003. When not explicitly set, the default value is determined by the target workbook file format.

### getTableName() {#getTableName--}

<b>@deprecated.</b> Please use the 'tableName' property instead. Gets or sets the name of the new PivotTable report.

```javascript
getTableName() : string;
```


**Remarks**

If not set , an automatic name will be set.

### setTableName(string) {#setTableName-string-}

<b>@deprecated.</b> Please use the 'tableName' property instead. Gets or sets the name of the new PivotTable report.

```javascript
setTableName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If not set , an automatic name will be set.

### getUseSameSource() {#getUseSameSource--}

<b>@deprecated.</b> Please use the 'useSameSource' property instead. Gets or sets a value indicating whether to share the same data source with existing pivot tables. Default value is true.

```javascript
getUseSameSource() : boolean;
```


**Remarks**

When set to true, multiple pivot tables can reuse one pivot cache to reduce memory consumption.

### setUseSameSource(boolean) {#setUseSameSource-boolean-}

<b>@deprecated.</b> Please use the 'useSameSource' property instead. Gets or sets a value indicating whether to share the same data source with existing pivot tables. Default value is true.

```javascript
setUseSameSource(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When set to true, multiple pivot tables can reuse one pivot cache to reduce memory consumption.

### isXlsClassic() {#isXlsClassic--}

<b>@deprecated.</b> Please use the 'isXlsClassic' property instead. Gets or sets a value indicating whether to create classic Excel 97-2003 style PivotTable.

```javascript
isXlsClassic() : boolean;
```


**Remarks**

Classic PivotTable uses legacy layout and formatting from Excel 97-2003. When not explicitly set, the default value is determined by the target workbook file format.

### setIsXlsClassic(boolean) {#setIsXlsClassic-boolean-}

<b>@deprecated.</b> Please use the 'isXlsClassic' property instead. Gets or sets a value indicating whether to create classic Excel 97-2003 style PivotTable.

```javascript
setIsXlsClassic(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Classic PivotTable uses legacy layout and formatting from Excel 97-2003. When not explicitly set, the default value is determined by the target workbook file format.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



