---
title: ExportTableOptions.DataTable
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Gets and sets the DataTable which columns data type is assigned
type: docs
url: /net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Gets and sets the DataTable which columns' data type is assigned.

```csharp
public DataTable DataTable { get; set; }
```

### Examples

```csharp
// Called: options.DataTable = data;
[Test]
        public void Property_DataTable()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];


            for (int i = 0; i &lt; 100; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    worksheet.Cells[i, j].PutValue(&quot;Test: &quot; + i.ToString() + &quot;,&quot; + j.ToString());


                }
            }

            DataTable data = new DataTable();
            data.Columns.Add(&quot;Name&quot;);
            data.Columns.Add(&quot;Num&quot;);
            data.Columns.Add(&quot;Date&quot;);


            int[] cols = { 2 }; // changing this value does nothing

            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = false;
            options.Indexes = new int[] { 2 };
            options.DataTable = data;
            // cells.ExportDataTable(dt, 0, new int[] { 0, 2 }, 3, true);
           // cells.ExportDataTable(0, 0, 3, 3, options);

            worksheet.Cells.ExportDataTable(0, 0, 100,1, options);

            Assert.AreEqual(data.Rows[0][0], &quot;Test: 0,2&quot;);

        


         

        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


