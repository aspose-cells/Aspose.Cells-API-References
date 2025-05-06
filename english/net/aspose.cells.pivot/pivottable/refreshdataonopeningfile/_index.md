---
title: PivotTable.RefreshDataOnOpeningFile
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether Refresh Data when Opening File
type: docs
url: /net/aspose.cells.pivot/pivottable/refreshdataonopeningfile/
---
## PivotTable.RefreshDataOnOpeningFile property

Indicates whether Refresh Data when Opening File.

```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```

### Examples

```csharp
// Called: table.RefreshDataOnOpeningFile = false;
[Test]
        public void Property_RefreshDataOnOpeningFile()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET44147And44175_&quot;;
            Workbook workbook = new Workbook(filePath + &quot;b.xlsx&quot;);
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Aspose.Cells.Pivot.PivotTableCollection collection = sheet.PivotTables;
                if (collection != null &amp;&amp; collection.Count &gt; 0)
                {
                    foreach (Aspose.Cells.Pivot.PivotTable table in collection)
                    {
                       

                        //Erro occurs because of this line
                        table.RefreshData();

                        table.CalculateData();
                        
                        table.RefreshDataOnOpeningFile = false;
                    }
                }
            }//foreach 
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;D8&quot;].StringValue, &quot;32&quot;);
            Assert.AreEqual(cells[&quot;E8&quot;].StringValue, &quot;3.2&quot;);
            Assert.AreEqual(cells[&quot;F8&quot;].StringValue, &quot;3.2&quot;);

            workbook.Save(Constants.PivotTableDestPath + @&quot;NET44147And44175b_out.xlsx&quot;);

            workbook = new Workbook(filePath + &quot;a.xlsx&quot;);
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Aspose.Cells.Pivot.PivotTableCollection collection = sheet.PivotTables;
                if (collection != null &amp;&amp; collection.Count &gt; 0)
                {
                    foreach (Aspose.Cells.Pivot.PivotTable table in collection)
                    {
                        

                        //Erro occurs because of this line
                        table.RefreshData();

                        table.CalculateData();
                       

                        table.RefreshDataOnOpeningFile = false;
                    }
                }
            }//foreach 
            cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;U15&quot;].StringValue, &quot;-34&quot;);
            Assert.AreEqual(cells[&quot;V15&quot;].StringValue, &quot;-68&quot;);
            Assert.AreEqual(cells[&quot;W15&quot;].StringValue, &quot;84&quot;);
            workbook.Save(Constants.PivotTableDestPath + @&quot;NET44147And44175a_out.xlsx&quot;);

            Workbook wb = new Workbook(filePath + &quot;Test-Template2.xlsx&quot;);
            Worksheet ws = wb.Worksheets[&quot;Data&quot;];
            ws.Cells.DeleteRows(20, 300);
            foreach (Worksheet sheet in wb.Worksheets)
            {
                Aspose.Cells.Pivot.PivotTableCollection collection = sheet.PivotTables;
                if (collection != null &amp;&amp; collection.Count &gt; 0)
                {
                    foreach (Aspose.Cells.Pivot.PivotTable table in collection)
                    {

                        //Erro occurs because of this line 
                        table.RefreshData();

                        table.CalculateData();
                        

                        table.RefreshDataOnOpeningFile = false;
                    }
                }
            }//foreach 
            cells = wb.Worksheets[1].Cells;
            Console.WriteLine(cells[&quot;N37&quot;].StringValue);
            Assert.AreEqual(cells[&quot;N37&quot;].StringValue, &quot; $19,904,150 &quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET44147And44175.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


