---
title: PivotTable.AddFieldToArea
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Adds the field to the specific area
type: docs
url: /net/aspose.cells.pivot/pivottable/addfieldtoarea/
---
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}

Adds the field to the specific area.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| fieldName | String | The name in the base fields. |

### Return Value

The field position in the specific fields.If there is no field named as it, return -1.

### Examples

```csharp
// Called: index = pivot.AddFieldToArea(PivotFieldType.Row, "H1");
public void PivotTable_Method_AddFieldToArea()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46360_";

    using (Workbook workbook = new Workbook(filePath + "TestPivot.xlsx"))
    {
        Worksheet sheet = workbook.Worksheets["Pivot"];
        int index = sheet.PivotTables.Add("='Data'!A1:E7", "A1", "MyPivot");
        PivotTable pivot = sheet.PivotTables[index];
        index = pivot.AddFieldToArea(PivotFieldType.Page, "H5");
        index = pivot.AddFieldToArea(PivotFieldType.Row, "H1");
        index = pivot.AddFieldToArea(PivotFieldType.Row, "H2");
        index = pivot.AddFieldToArea(PivotFieldType.Data, "H4");
        index = pivot.AddFieldToArea(PivotFieldType.Data, "H3");
        pivot.AddFieldToArea(PivotFieldType.Column, pivot.DataField);
        pivot.RefreshData();
        pivot.CalculateRange();
        pivot.CalculateData();
        workbook.Save(CreateFolder(filePath) + "out.xlsx");
    }
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}

Adds the field to the specific area.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| baseFieldIndex | Int32 | The field index in the base fields. |

### Return Value

The field position in the specific fields.

### Examples

```csharp
// Called: pivotTable.AddFieldToArea(PivotFieldType.Data, 2);
public void PivotTable_Method_AddFieldToArea()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "Net1.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];

    // Add a Pivot Table
    int pivotTableIndex = worksheet.PivotTables.Add("=A1:C133", "J1", "PivotTable1", false, false);
    PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

    // Set the row fields
    pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
    //  pivotTable.AddFieldToArea(PivotFieldType.Row, 1);

    // Set the data field
    pivotTable.AddFieldToArea(PivotFieldType.Data, 2);
    Assert.AreEqual(PivotTableStyleType.PivotTableStyleLight16, pivotTable.PivotTableStyleType);
    Assert.IsFalse(pivotTable.ShowValuesRow);
    Assert.IsFalse(pivotTable.IsExcel2003Compatible);
    // Save the workbook with the Pivot Table
    workbook.Save(Constants.PivotTableDestPath + "out_net.xlsx");
    ;
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}

Adds the field to the specific area.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the fields area type. |
| pivotField | PivotField | the field in the base fields. |

### Return Value

the field position in the specific fields.

### Examples

```csharp
// Called: pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
public void PivotTable_Method_AddFieldToArea()
{
    Workbook workbook = new Workbook(Constants.openPivottablePath + "Bad.xlsx");

    Worksheet pivotSheet = workbook.Worksheets.Add("PivotData");
    pivotSheet.Name = "Summarize";

    PivotTableCollection pivotTables = pivotSheet.PivotTables;
    string source = String.Format("='Source Data'!A1:D5");
    int index = pivotTables.Add(source, "A1", "PivotTable");
    PivotTable pTable = pivotTables[index];

    pTable.IsAutoFormat = true;
    pTable.AutoFormatType = PivotTableAutoFormatType.Classic;

    pTable.AddFieldToArea(PivotFieldType.Row, 0);
    pTable.AddFieldToArea(PivotFieldType.Row, 1);

    pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
    pTable.DataFields[0].Function = ConsolidationFunction.Sum;
    pTable.DataFields[0].NumberFormat = "$0.00";

    if (pTable.DataField != null)
    {
        pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
    }

    workbook.Save(Constants.savePivottablePath + "t.xlsx");
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


