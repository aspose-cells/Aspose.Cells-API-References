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
// Called: var dataFields = pivotTable.Fields(PivotFieldType.Data);
[Test]
        public void Method_PivotFieldType_()
        {
            string filePath = Constants.PivotTableSourcePath  + @&quot;NET44304_&quot;;
            Workbook wb = new Workbook(filePath + &quot;sample.xlsx&quot;);
            Worksheet ws = wb.Worksheets[&quot;Pivot Sheet&quot;];

            PivotTable pivotTable = ws.PivotTables[0];

            pivotTable.IsExcel2003Compatible = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            var dataFields = pivotTable.Fields(PivotFieldType.Data);

            for (int i = 255; i &lt; dataFields.Count; i++)
            {
                var displayName = dataFields[i].DisplayName;

                Cell cell = pivotTable.GetCellByDisplayName(displayName);

                if (cell == null)
                {
                    Assert.Fail(&quot;find null via PivotField.DisplayName&quot;);
                    Console.WriteLine(displayName + &quot;----Null&quot;);
                }
                else
                {
                    Console.WriteLine(displayName + &quot;----&quot; + cell.Name);
                }
            }
            wb.Save(Constants.PivotTableDestPath + @&quot;NET44304.xlsx&quot;);

            wb = new Workbook(Constants.PivotTableDestPath + @&quot;NET44304.xlsx&quot;);
            pivotTable = wb.Worksheets[&quot;Pivot Sheet&quot;].PivotTables[0];
            dataFields = pivotTable.Fields(PivotFieldType.Data);
            for (int i = 255; i &lt; dataFields.Count; i++)
            {
                var displayName = dataFields[i].DisplayName;

                Cell cell = pivotTable.GetCellByDisplayName(displayName);

                if (cell == null)
                {
                    Assert.Fail(&quot;find null via PivotField.DisplayName&quot;);
                    Console.WriteLine(displayName + &quot;----Null&quot;);
                }
                else
                {
                    Console.WriteLine(displayName + &quot;----&quot; + cell.Name);
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


