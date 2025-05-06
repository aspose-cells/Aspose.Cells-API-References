---
title: PivotTable.ShowValuesRow
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether showing values row
type: docs
url: /net/aspose.cells.pivot/pivottable/showvaluesrow/
---
## PivotTable.ShowValuesRow property

Indicates whether showing values row.

```csharp
public bool ShowValuesRow { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;After &amp;quot; + table.ShowValuesRow);
[Test]
        public void Property_ShowValuesRow()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46650_&quot;;

            Workbook workbook = new Workbook(filePath + @&quot;origin.xlsx&quot;);

            foreach (Worksheet sheet in workbook.Worksheets)
            {
                foreach (PivotTable table in sheet.PivotTables)
                {
                    Console.WriteLine(&quot;Before &quot; + table.ShowValuesRow);
                    table.ShowValuesRow = false;
                    Console.WriteLine(&quot;After &quot; + table.ShowValuesRow);
                }
                sheet.RefreshPivotTables();
            }

            workbook.Save(CreateFolder(filePath) + @&quot;out.xlsx&quot;, Aspose.Cells.SaveFormat.Xlsx);

            workbook = new Workbook(CreateFolder(filePath) + @&quot;out.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PivotTables[0].ShowValuesRow, false);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


