---
title: PivotTable.IsExcel2003Compatible
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable if true a string must be less than or equal to 255 characters so if the string is greater than 255 characters it will be truncated. if false a string will not have the aforementioned restriction. The default value is true
type: docs
url: /net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### Examples

```csharp
// Called: pivotTable.IsExcel2003Compatible = false;
[Test]
        public void Property_IsExcel2003Compatible()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA41908_&quot;;

            Workbook wb = new Workbook(filePath + &quot;pivot_table.xlsx&quot;);
            wb.CalculateFormula(true);
            Worksheet sheet = wb.Worksheets[1];
            //Access cell &quot;A1&quot; in the sheet. 
            Cells cells = sheet.Cells;
            Cell cell = cells[&quot;A3&quot;];
            cell.Value = &quot;FooBar&quot;;
            cell = cells[&quot;B3&quot;];
            cell.Value = &quot;very long text 1. very long text 2. very long text 3. very long text 4. very long text 5. very long text 6. very long text 7. very long text 8. very long text 9. very long text 10. very long text 11. very long text 12. very long text 13. very long text 14. very long text 15. very long text 16. very long text 17. very long text 18. very long text 19. very long text 20.&quot;;
            cell = cells[&quot;C3&quot;];
            cell.Value = &quot;closed&quot;;
            cell = cells[&quot;D3&quot;];
            cell.Value = &quot;2016/07/21&quot;;

            sheet = wb.Worksheets[0];
            //sheet.autoFitColumns(); 
            PivotTable pivotTable = sheet.PivotTables[0];
            pivotTable.IsExcel2003Compatible = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            Assert.Greater(sheet.Cells[&quot;B6&quot;].StringValue.Length, 260);
            //pivotTable.setRefreshDataOnOpeningFile(true);
            wb.Save(Constants.PivotTableDestPath + @&quot;JAVA41908.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


