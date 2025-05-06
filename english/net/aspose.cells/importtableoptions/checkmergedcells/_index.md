---
title: ImportTableOptions.CheckMergedCells
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether checking merged cells
type: docs
url: /net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Indicates whether checking merged cells.

```csharp
public bool CheckMergedCells { get; set; }
```

### Examples

```csharp
// Called: options.CheckMergedCells = true;
[Test]
        public void Property_CheckMergedCells()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet46711.xlsx&quot;);
            List&lt;Customer&gt; customerList = new List&lt;Customer&gt;();

            //Creating collection for test items
            for (int i = 0; i &lt; 5; i++)
            {
                Customer customer = new Customer
                {
                    CustomerId = i,
                    Name = &quot;Customer&quot; + i
                };
                customerList.Add(customer);
            }
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = false;
            options.TotalRows = customerList.Count;
            options.InsertRows = true;
            options.DateFormat = &quot;dd/mm/yyyy&quot;;
            options.ConvertNumericData = true;
            options.CheckMergedCells = true;
            //Insert data to excell
            wb.Worksheets[0].Cells.ImportCustomObjects((ICollection)customerList, 1, 0, options);
            Cell d4 = wb.Worksheets[0].Cells[&quot;D4&quot;];
            Assert.AreEqual(d4.StringValue, &quot;Customer2&quot;);
            Assert.IsTrue(d4.IsMerged);
            wb.Save(Constants.destPath + &quot;CellsNet46711.xlsx&quot;, Aspose.Cells.SaveFormat.Xlsx);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


