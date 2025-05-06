---
title: Name.SheetIndex
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates this name belongs to Workbook or Worksheet. 0  Global name otherwise index to sheet onebased
type: docs
url: /net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)

```csharp
public int SheetIndex { get; set; }
```

### Examples

```csharp
// Called: if (wkCopy.Worksheets.Names[i].SheetIndex == idx + 1)
[Test]
        public void Property_SheetIndex()
        {
            Workbook wk1 = new Workbook(Constants.sourcePath + &quot;CellsNet44259.xls&quot;);
            Workbook wkCopy = new Workbook(FileFormatType.Xlsx);

            wk1.Worksheets.Add(&quot;PrimoSheet&quot;);
            wk1.Worksheets[wk1.Worksheets.Count - 1].MoveTo(1);
            wk1.Worksheets[1].Copy(wk1.Worksheets[0]);
            wkCopy.Copy(wk1);

            int idx = wkCopy.Worksheets[&quot;ub2&quot;].Index;
            for (int i = 0; i &lt; wkCopy.Worksheets.Names.Count; i++)
            {
                if (wkCopy.Worksheets.Names[i].SheetIndex == idx + 1)
                {
                    wkCopy.Worksheets.Names[i].RefersTo = &quot;&quot;;
                    wkCopy.Worksheets.Names[i].IsVisible = false;
                }
            }

            wkCopy.Worksheets.RemoveAt(&quot;ub2&quot;);

            Cell c = wkCopy.Worksheets[0].Cells.Find(&quot;RDB&quot;, null, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
            while (c != null)
            {
                c.Formula = &quot;&quot;;
                c = wkCopy.Worksheets[0].Cells.Find(&quot;RDB&quot;, c, new FindOptions()
                { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
            }

            wkCopy.Worksheets.ActiveSheetIndex = 0;
            Util.SaveManCheck(wkCopy, &quot;Shape&quot;, &quot;CellsNet44259.xls&quot;);
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


