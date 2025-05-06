---
title: WorksheetCollection.SortNames
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Sorts the defined names
type: docs
url: /net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Sorts the defined names.

```csharp
public void SortNames()
```

### Remarks

If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving

### Examples

```csharp
// Called: wb.Worksheets.SortNames();
[Test]
        public void Method_SortNames()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.CreateRange(0, 0, 2, 2).Name = &quot;testname3&quot;;
            cells.CreateRange(2, 0, 2, 2).Name = &quot;testname0&quot;;
            cells.CreateRange(4, 0, 2, 2).Name = &quot;testname1&quot;;
            cells.CreateRange(6, 0, 2, 2).Name = &quot;testname2&quot;;

            string fml = &quot;=testname1-testname2*testname3/testname0&quot;;
            cells[0, 2].SetSharedFormula(fml, 106, 1);
            wb.Worksheets.SortNames();
            for (int i = 0; i &lt; 106; i++)
            {
                Assert.AreEqual(fml, cells[i, 2].Formula, &quot;rowindex=&quot; + i);
            }
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


