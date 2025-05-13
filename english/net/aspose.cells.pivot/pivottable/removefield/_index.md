---
title: PivotTable.RemoveField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Removes a field from specific field area
type: docs
url: /net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Removes a field from specific field area

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| fieldName | String | The name in the base fields. |

### Examples

```csharp
// Called: pt.RemoveField(PivotFieldType.Data, "c");
public void PivotTable_Method_RemoveField()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets["Sheet3"].PivotTables[0];
    pt.RemoveField(PivotFieldType.Data, "c");
    pt.CalculateData();
    Assert.AreEqual("0", workbook.Worksheets["Sheet3"].Cells["C4"].StringValue);
    pt = workbook.Worksheets["Sheet1"].PivotTables[0];
    pt.RemoveField(PivotFieldType.Data, "c");
    pt.CalculateData();
    Assert.AreEqual("0", workbook.Worksheets["Sheet1"].Cells["H11"].StringValue);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Removes a field from specific field area

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| baseFieldIndex | Int32 | The field index in the base fields. |

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Remove field from specific field area

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the fields area type. |
| pivotField | PivotField | the field in the base fields. |

### Examples

```csharp
// Called: wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Column, wb.Worksheets[0].PivotTables[0].ColumnFields[0]);
public void PivotTable_Method_RemoveField()
{
    var wb = new Workbook(Constants.openPivottablePath + "TestFile.xlsx");
    wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Data, wb.Worksheets[0].PivotTables[0].DataFields[0]);
    wb.Save(Constants.savePivottablePath + "example.xlsx");


    wb = new Workbook(Constants.openPivottablePath + "example.xlsx");
    wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Column, wb.Worksheets[0].PivotTables[0].ColumnFields[0]);
    wb.Save(Constants.savePivottablePath + "example.xlsx");
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


