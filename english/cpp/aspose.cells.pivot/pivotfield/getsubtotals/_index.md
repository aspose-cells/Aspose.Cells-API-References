---
title: Aspose::Cells::Pivot::PivotField::GetSubtotals method
linktitle: GetSubtotals
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotField::GetSubtotals method. Indicates whether to show specified subtotal for this pivot field in C++.'
type: docs
weight: 3200
url: /cpp/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField::GetSubtotals(PivotFieldSubtotalType) method


Indicates whether to show specified subtotal for this pivot field.

```cpp
bool Aspose::Cells::Pivot::PivotField::GetSubtotals(PivotFieldSubtotalType subtotalType)
```


| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Subtotal type. |

## ReturnValue

Returns whether showing specified subtotal.

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotField::GetSubtotals() method


Gets or sets the subtotals of the field. Only for [Row](../../../aspose.cells/row/) or [Column](../../../aspose.cells/column/) pivot field.

```cpp
PivotFieldSubtotalType Aspose::Cells::Pivot::PivotField::GetSubtotals()
```


## Examples


```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 0).PutValue(u"fruit");
cells.Get(1, 0).PutValue(u"grape");
cells.Get(2, 0).PutValue(u"blueberry");
cells.Get(3, 0).PutValue(u"kiwi");
cells.Get(4, 0).PutValue(u"cherry");
cells.Get(5, 0).PutValue(u"grape");
cells.Get(6, 0).PutValue(u"blueberry");
cells.Get(7, 0).PutValue(u"kiwi");
cells.Get(8, 0).PutValue(u"cherry");

cells.Get(0, 1).PutValue(u"year");
cells.Get(1, 1).PutValue(2020);
cells.Get(2, 1).PutValue(2020);
cells.Get(3, 1).PutValue(2020);
cells.Get(4, 1).PutValue(2020);
cells.Get(5, 1).PutValue(2021);
cells.Get(6, 1).PutValue(2021);
cells.Get(7, 1).PutValue(2021);
cells.Get(8, 1).PutValue(2021);

cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);
cells.Get(5, 2).PutValue(90);
cells.Get(6, 2).PutValue(100);
cells.Get(7, 2).PutValue(110);
cells.Get(8, 2).PutValue(120);

PivotTableCollection pivots = sheet.GetPivotTables();

int pivotIndex = pivots.Add(u"=Sheet1!A1:C9", u"A12", u"TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"year");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");

pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);

//Change PivotField's attributes
PivotField rowField = pivot.GetRowFields().Get(0);
rowField.SetDisplayName(u"custom display name");

pivot.RefreshData();
pivot.CalculateData();

PivotFieldSubtotalType type = rowField.GetSubtotals();

book.Save("out.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* Class [PivotField](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
