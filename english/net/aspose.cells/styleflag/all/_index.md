---
title: StyleFlag.All
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. All properties will be applied
type: docs
url: /net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

All properties will be applied.

```csharp
public bool All { get; set; }
```

### Examples

```csharp
// Called: f.All = true;
[Test]
        public void Property_All()
        {
            var wb = new Workbook();
            var ws = wb.Worksheets[0];
            var s = wb.CreateStyle();
            var f = new StyleFlag();
            s.Font.Name = &quot;Tahoma&quot;;
            s.Font.Size = 7;
            f.All = true;
            ws.Cells.ApplyStyle(s, f);
            ws.Cells.StandardHeight = 12.75;
            ws.Cells[0, 0].PutValue(&quot;Value1&quot;);
            ws.Cells[1, 0].PutValue(&quot;Value2&quot;);
            ws.Cells[2, 0].PutValue(&quot;Value3&quot;);
            ws.AutoFitColumns();
            Assert.AreEqual(ws.Cells.Rows[0].IsHeightMatched, false);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


