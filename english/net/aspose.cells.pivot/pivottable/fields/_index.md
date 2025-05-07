---
title: PivotTable.Fields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the specific fields by the field type
type: docs
url: /net/aspose.cells.pivot/pivottable/fields/
---
## PivotTable.Fields method

Gets the specific fields by the field type.

```csharp
[Obsolete("Use PivotField.GetFields() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldCollection Fields(PivotFieldType fieldType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the field type. |

### Return Value

the specific field collection

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GetFields() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: dataFields = pivotTable.Fields(PivotFieldType.Data);
[Test]
        public void Method_PivotFieldType_()
        {
            string filePath = Constants.PivotTableSourcePath  + @"NET44304_";
            Workbook wb = new Workbook(filePath + "sample.xlsx");
            Worksheet ws = wb.Worksheets["Pivot Sheet"];

            PivotTable pivotTable = ws.PivotTables[0];

            pivotTable.IsExcel2003Compatible = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            var dataFields = pivotTable.Fields(PivotFieldType.Data);

            for (int i = 255; i < dataFields.Count; i++)
            {
                var displayName = dataFields[i].DisplayName;

                Cell cell = pivotTable.GetCellByDisplayName(displayName);

                if (cell == null)
                {
                    Assert.Fail("find null via PivotField.DisplayName");
                    Console.WriteLine(displayName + "----Null");
                }
                else
                {
                    Console.WriteLine(displayName + "----" + cell.Name);
                }
            }
            wb.Save(Constants.PivotTableDestPath + @"NET44304.xlsx");

            wb = new Workbook(Constants.PivotTableDestPath + @"NET44304.xlsx");
            pivotTable = wb.Worksheets["Pivot Sheet"].PivotTables[0];
            dataFields = pivotTable.Fields(PivotFieldType.Data);
            for (int i = 255; i < dataFields.Count; i++)
            {
                var displayName = dataFields[i].DisplayName;

                Cell cell = pivotTable.GetCellByDisplayName(displayName);

                if (cell == null)
                {
                    Assert.Fail("find null via PivotField.DisplayName");
                    Console.WriteLine(displayName + "----Null");
                }
                else
                {
                    Console.WriteLine(displayName + "----" + cell.Name);
                }
            }
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


