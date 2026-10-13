---
title: PivotFieldTop10AutoShowSettings
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the Top 10 AutoShow settings for a pivot field.
type: docs
url: /javascript-cpp/pivotfieldtop10autoshowsettings/
---

## PivotFieldTop10AutoShowSettings class

Represents the Top 10 AutoShow settings for a pivot field.

```javascript
class PivotFieldTop10AutoShowSettings;
```

### Remarks
In xls : Implementing top 10 filters in Xls through Top 10 AutoShow In ooxml files: The underlying ooxml file format supports Top10 AutoShow, but Excel 2007 and later user interface only provides access via Top10 filter. If XLS compatibility is not required, it is recommended to use Top10 filter instead.

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isAutoShow](#isAutoShow--)| boolean | Indicates whether an "Top 10 AutoShow" filter is applied to this field. |
| [isTop](#isTop--)| boolean | Indicates whether the specified PivotTable field is autoshown ascending. |
| [autoShowCount](#autoShowCount--)| number | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [rankBy](#rankBy--)| number | Specifies the index of data field for AutoShow ranking. Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |


### isAutoShow {#isAutoShow--}

Indicates whether an "Top 10 AutoShow" filter is applied to this field.

```javascript
isAutoShow : boolean;
```


### isTop {#isTop--}

Indicates whether the specified PivotTable field is autoshown ascending.

```javascript
isTop : boolean;
```


### autoShowCount {#autoShowCount--}

Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

```javascript
autoShowCount : number;
```


### rankBy {#rankBy--}

Specifies the index of data field for AutoShow ranking. Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

```javascript
rankBy : number;
```



