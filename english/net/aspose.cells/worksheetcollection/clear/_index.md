---
title: WorksheetCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Clear all worksheets
type: docs
url: /net/aspose.cells/worksheetcollection/clear/
---
## WorksheetCollection.Clear method

Clear all worksheets.

```csharp
public void Clear()
```

### Remarks

A workbook must contains a worksheet.

### Examples

```csharp
// Called: wb.Worksheets.Clear();
[Test]
        public void Method_Clear()
        {
            Console.WriteLine(&quot;Method_Clear()&quot;);
            string outfn = Constants.destPath + &quot;Test_VertAlign_out.xlsx&quot;;

            Workbook wb = new Workbook();

            wb.Worksheets.Clear();

            Worksheet ws = wb.Worksheets.Add(&quot;Sheet&quot;);

            Style s = wb.CreateStyle();

            s.Name = &quot;NewStyle&quot;;

            s.Font.Underline = FontUnderlineType.Single;

            s.BackgroundColor = Color.Blue;

            s.VerticalAlignment = TextAlignmentType.Center;

            Cells cells = ws.Cells;

            Cell c = cells[&quot;F2&quot;];

            c.PutValue(&quot;Text&quot;);

            c.SetStyle(s);

            wb.Save(outfn);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


