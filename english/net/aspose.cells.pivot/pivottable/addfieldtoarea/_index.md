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
// Called: pivotTable.AddFieldToArea(PivotFieldType.Row, column);
private static void Method_String_(Workbook workbook, List<string> columns)
        {
            var pivotSheet = workbook.Worksheets.Add("Pivot1");
            var pivotTableIndex = pivotSheet.PivotTables.Add(string.Format("'{0}'!{1}", "Pivot1", "Data0"), "A5", "Pivot");
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            foreach (var column in columns)
            {
                pivotTable.AddFieldToArea(PivotFieldType.Row, column);
            }
            pivotTable.CalculateData();

            foreach (var column in columns)
            {
                var cell = pivotTable.GetCellByDisplayName(column);
                if (cell == null)
                    continue;
                var style = new Style(); // this used to work in 20.04 but causes corruption starting with 20.06
                                         // style.BackgroundColor = Color.Red;
                pivotTable.Format(cell.Row, cell.Column, style);
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
// Called: pt.AddFieldToArea(PivotFieldType.Data, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.openPivottablePath + "SR3.xls");

            Worksheet ws = workbook.Worksheets[1];
            PivotTable pt = ws.PivotTables[(ws.PivotTables.Add("'Grid Results'!B4:E8", 2, 0, "Hello"))];
            pt.AddFieldToArea(PivotFieldType.Row, 1);
            pt.AddFieldToArea(PivotFieldType.Data, 0);
            pt.RowFields[0].IsAutoSort = true;
            workbook.Save(Constants.savePivottablePath + "c.xls");
            //workbook.Save("D:\\c.xlsx", FileFormatType.Xlsx);
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
// Called: pivot.AddFieldToArea(PivotFieldType.Column, pivot.DataField);
[Test]
        public void Method_PivotField_()
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
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


