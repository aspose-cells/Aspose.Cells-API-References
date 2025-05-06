---
title: Cell.ToString
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Returns a string represents the current Cell object
type: docs
url: /net/aspose.cells/cell/tostring/
---
## Cell.ToString method

Returns a string represents the current Cell object.

```csharp
public override string ToString()
```

### Examples

```csharp
// Called: colHeader = worksheet.Cells[0, intCol].ToString();
[Test]
        public void Method_ToString()
        {
            bool cont = true;
            while (cont)
            {
                string FilePath = Constants.sourcePath + &quot;CellsNet41204.xlsx&quot;;
                Aspose.Cells.LoadOptions Loadoptions = new Aspose.Cells.LoadOptions(LoadFormat.Xlsx);
                Workbook workbook = new Workbook(FilePath, Loadoptions);
                Worksheet worksheet = workbook.Worksheets[0];
                if (worksheet != null)
                {
                    int totalColumnsLoaded = 0;
                    int maxCol = 0;
                    string colHeader = &quot;&quot;;
                    try
                    {
                        maxCol = worksheet.Cells.MaxColumn;

                        for (int intCol = 0; intCol &lt; maxCol; intCol += 2)
                        {

                            if ((worksheet.Cells[0, intCol].ToString()) != null)
                            {
                                int maxRowInCol = worksheet.Cells.GetLastDataRow(intCol);
                                colHeader = worksheet.Cells[0, intCol].ToString();
                                if (colHeader != null)
                                {
                                    DataTable dataTable = new DataTable();
                                    ExportTableOptions option = new ExportTableOptions();
                                    option.SkipErrorValue = true;
                                    option.ExportColumnName = true;
                                    //extract data from excel and fill in data table for each of the column

                                    //It throws an error for every column except for the first column when we use ExportDataTable with 5th argurment as ExportTableOptions. It loads the first column correctly.
                                    dataTable = worksheet.Cells.ExportDataTable(1, intCol, maxRowInCol, 2, option);

                                    //But if we use ExportDataTable with 5th argurment as bool Export Column Name then it properly iterates through each of the column and gives the desired resutls.
                                    // dataTable = worksheet.Cells.ExportDataTableAsString(1, intCol, maxRowInCol, 2, true);

                                    totalColumnsLoaded++;
                                }
                            }
                        }
                    }
                    //catch (Exception Ex)
                    //{
                    //    Console.WriteLine(&quot;Exception Thrown:&quot; + Ex.Message);

                    //}
                    finally
                    {

                        Console.WriteLine(&quot;TotalColumns Loaded:&quot; + totalColumnsLoaded);
                        cont = false;
                    }
                }
            }

        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


