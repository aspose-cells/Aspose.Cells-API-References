---
title: Cells.MaxDisplayRange
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the max range which includes data merged cells and shapes
type: docs
url: /net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Gets the max range which includes data, merged cells and shapes.

```csharp
public Range MaxDisplayRange { get; }
```

### Remarks

Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.

### Examples

```csharp
// Called: Aspose.Cells.Range dataRange = sheet.Cells.MaxDisplayRange;
private DataTable Property_MaxDisplayRange(ExternalConnection dataSource, string filePath)
        {
            DBConnection conn = (DBConnection)dataSource;
            //The data file path of the external connection is related to the local, and the current directory file is read directly here.
            //Workbook dataBook = new Workbook(conn.SourceFile);
            Workbook dataBook = new Workbook(filePath + &quot;data.xlsx&quot;);
            string sheetName = conn.Command.Replace(&quot;$&quot;, &quot;&quot;);
            Worksheet sheet = dataBook.Worksheets[sheetName];
            Aspose.Cells.Range dataRange = sheet.Cells.MaxDisplayRange;


            DataTable table = new DataTable();


            int endRow = dataRange.FirstRow + dataRange.RowCount;
            int endCol = dataRange.FirstColumn + dataRange.ColumnCount;

            //Set column name and data type.
            //You can obtain the header and data type from an external data source.
            table.Columns.Add(new DataColumn(&quot;fruit&quot;, typeof(string)));
            table.Columns.Add(new DataColumn(&quot;country&quot;, typeof(string)));
            table.Columns.Add(new DataColumn(&quot;amount&quot;, typeof(int)));

            //Add data. The external data source of the example is an excel file, so we directly get data from the worksheet.
            for (int r = dataRange.FirstRow + 1; r &lt; endRow; r++)
            {
                DataRow row = table.NewRow();
                table.Rows.Add(row);
                int index = 0;
                for (int c = dataRange.FirstColumn; c &lt; endCol; c++)
                {
                    object temp = sheet.Cells[r, c].Value;
                    //modify data for test, change &quot;grape&quot; to &quot;grape_modify&quot;.
                    if (temp is string &amp;&amp; (string)temp == &quot;grape&quot;)
                    {
                        temp = &quot;grape_modify&quot;;
                    }
                    row[index++] = temp;
                }

            }

            return table;
        }
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


