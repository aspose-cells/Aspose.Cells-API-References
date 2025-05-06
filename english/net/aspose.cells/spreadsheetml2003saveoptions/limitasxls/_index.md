---
title: SpreadsheetML2003SaveOptions.LimitAsXls
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetML2003SaveOptions property. Limit as xls the max row index is 65535 and the max column index is 255
type: docs
url: /net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Limit as xls, the max row index is 65535 and the max column index is 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Examples

```csharp
// Called: LimitAsXls = true
[Test]
        public void Property_LimitAsXls()
        {
            caseName = &quot;testCreateRange_022&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange(&quot;IV65536&quot;, &quot;IV65536&quot;);  //=Sheet1!$1:$65536
            range.Name = &quot;testRange&quot;;

            checkCreateRange_022(workbook);
            workbook.Save(Constants.destPath + &quot;testCreateRange.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testCreateRange.xls&quot;);
            checkCreateRange_022(workbook);
            workbook.Save(Constants.destPath + &quot;testCreateRange.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testCreateRange.xlsx&quot;);
            checkCreateRange_022(workbook);
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            workbook.Save(Constants.destPath + &quot;testCreateRange.xml&quot;, saveOptions);
            workbook = new Workbook(Constants.destPath + &quot;testCreateRange.xml&quot;);
            checkCreateRange_022(workbook);
            workbook.Save(Constants.destPath + &quot;testCreateRange.xls&quot;);  
        }
```

### See Also

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


