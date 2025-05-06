---
title: LoadOptions.LightCellsDataHandler
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. The data handler for processing cells data when reading template file
type: docs
url: /net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

The data handler for processing cells data when reading template file.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Examples

```csharp
// Called: opts.LightCellsDataHandler = v;
private void Property_LightCellsDataHandler(string file, int startRow, int startColumn, int endRow, int endColumn,
            string sheetName, SaveFormat[] otherFmts)
        {
            Console.WriteLine(&quot;Processing &quot; + file + &quot;...&quot;);
            LoadOptions opts = new LoadOptions();
            Workbook wbBase = new Workbook(file);
            LightCellsDataHandlerVisitCells v = new LightCellsDataHandlerVisitCells(file + &quot;: &quot;,
                wbBase, startRow, startColumn, endRow, endColumn, sheetName);
            opts.LightCellsDataHandler = v;
            Workbook wb = new Workbook(file, opts);
            string err = v.GetError();
            wb.Dispose();
            if (err != null)
            {
                Assert.Fail(err);
            }
            if (otherFmts != null)
            {
                MemoryStream ms = new MemoryStream();
                foreach (SaveFormat sf in otherFmts)
                {
                    Console.WriteLine(&quot;Processing as &quot; + sf + &quot;...&quot;);
                    wb = new Workbook(file);
                    wb.Save(ms, sf);
                    wb.Dispose();
                    ms.Seek(0, SeekOrigin.Begin);
                    Property_LightCellsDataHandler(ms, startRow, startColumn, endRow, endColumn,
                        sheetName, wbBase, file + &quot;.&quot; + sf);
                    ms.SetLength(0);
                }
            }
        }
```

### See Also

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


