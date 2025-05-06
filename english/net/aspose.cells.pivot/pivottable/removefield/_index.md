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
// Called: pt.RemoveField(PivotFieldType.Data, &amp;quot;c&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSJAVA45392.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[&quot;Sheet3&quot;].PivotTables[0];
            pt.RemoveField(PivotFieldType.Data, &quot;c&quot;);
            pt.CalculateData();
            Assert.AreEqual(&quot;0&quot;, workbook.Worksheets[&quot;Sheet3&quot;].Cells[&quot;C4&quot;].StringValue);
            pt = workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[0];
            pt.RemoveField(PivotFieldType.Data, &quot;c&quot;);
            pt.CalculateData();
            Assert.AreEqual(&quot;0&quot;, workbook.Worksheets[&quot;Sheet1&quot;].Cells[&quot;H11&quot;].StringValue);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSJAVA45392.xlsx&quot;);
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
// Called: wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Data, wb.Worksheets[0].PivotTables[0].DataFields[0]);
[Test]
        public void Method_PivotField_()
        {
            var wb = new Workbook(Constants.openPivottablePath + &quot;TestFile.xlsx&quot;);
            wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Data, wb.Worksheets[0].PivotTables[0].DataFields[0]);
            wb.Save(Constants.savePivottablePath + &quot;29234.xlsx&quot;);


            wb = new Workbook(Constants.openPivottablePath + &quot;201101-Mock+BudgetOriginatorJobCodeDetailsReport-1(1).xlsx&quot;);
            wb.Worksheets[0].PivotTables[0].RemoveField(PivotFieldType.Column, wb.Worksheets[0].PivotTables[0].ColumnFields[0]);
            wb.Save(Constants.savePivottablePath + &quot;201101-Mock+BudgetOriginatorJobCodeDetailsReport-1(1).xlsx&quot;);
        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


