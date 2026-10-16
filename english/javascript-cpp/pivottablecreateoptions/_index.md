---
title: PivotTableCreateOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Options for creating a new PivotTable.
type: docs
url: /javascript-cpp/pivottablecreateoptions/
---

## PivotTableCreateOptions class

Options for creating a new PivotTable.

```javascript
class PivotTableCreateOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [tableName](#tableName--)| string | Gets or sets the name of the new PivotTable report. |
| [useSameSource](#useSameSource--)| boolean | Gets or sets a value indicating whether to share the same data source with existing pivot tables. Default value is true. |
| [isXlsClassic](#isXlsClassic--)| boolean | Gets or sets a value indicating whether to create classic Excel 97-2003 style PivotTable. |


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


