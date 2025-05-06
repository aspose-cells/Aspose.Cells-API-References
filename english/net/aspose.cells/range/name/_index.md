---
title: Range.Name
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets or sets the name of the range
type: docs
url: /net/aspose.cells/range/name/
---
## Range.Name property

Gets or sets the name of the range.

```csharp
public string Name { get; set; }
```

### Remarks

Named range is supported. For example,

range.Name = "Sheet1!MyRange";

### Examples

```csharp
// Called: range.Name = &amp;quot;testRange&amp;quot;;
[Test]
        public void Property_Name()
        {
            caseName = &quot;testCreateRange_Excel2007_001&quot;;
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange(0, 16384, true);
            range.Name = &quot;testRange&quot;;

            checkCreateRange_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + &quot;testCreateRange.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testCreateRange.xlsx&quot;);
            checkCreateRange_Excel2007_001(workbook);
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            workbook.Save(Constants.destPath + &quot;testCreateRange.xml&quot;, saveOptions);
            workbook = new Workbook(Constants.destPath + &quot;testCreateRange.xml&quot;);
            workbook.Save(Constants.destPath + &quot;testCreateRange.xls&quot;);  
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


