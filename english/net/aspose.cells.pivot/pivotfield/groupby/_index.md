---
title: PivotField.GroupBy
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Automatically group the field with internal
type: docs
url: /net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_3}

Automatically group the field with internal

```csharp
public void GroupBy(double interval, bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| interval | Double | The internal of group. Automatic value will be assigned if it's zero, |
| newField | Boolean | Indicates whether adding a new field to the pivottable. |

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_2}

Group the file by the date group types.

```csharp
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start datetime |
| end | DateTime | The end of datetime |
| groups | PivotGroupByType[] | Group types |
| interval | Double | The interval |
| firstAsNewField | Boolean | Indicates whether adding a new field to the pivottable. Only for the first group item. |

### Return Value

False means this field could not be grouped by date time.

### See Also

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_1}

Group the file by number.

```csharp
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | Double | The start value |
| end | Double | The end of value |
| interval | Double | The interval |
| newField | Boolean | Indicates whether adding a new field to the pivottable |

### Return Value

False means this field could not be grouped by date time.

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Custom group the field.

```csharp
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | The custom group items. |
| newField | Boolean | Indicates whether adding a new field to the pivottable |

### Return Value

False means this field could not be grouped by date time.

### See Also

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


