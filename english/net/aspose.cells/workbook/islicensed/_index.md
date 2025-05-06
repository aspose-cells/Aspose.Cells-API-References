---
title: Workbook.IsLicensed
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Indicates whether license is set
type: docs
url: /net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Indicates whether license is set.

```csharp
public bool IsLicensed { get; }
```

### Examples

```csharp
// Called: VerifyLoadFilter(ms, wb.IsLicensed ? 2 : 4);
[Test]
        public void Property_IsLicensed()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Name = &quot;st0&quot;;
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;abc&quot;);
            wb.Worksheets.Add(&quot;st1&quot;);
            wb.BuiltInDocumentProperties.Author = &quot;Aspose.Cells&quot;;
            wb.CustomDocumentProperties.Add(&quot;MyCustomProp&quot;, &quot;MyVal&quot;);
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
            VerifyLoadFilter(ms, wb.IsLicensed ? 2 : 3);
            ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            VerifyLoadFilter(ms, wb.IsLicensed ? 2 : 4);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


