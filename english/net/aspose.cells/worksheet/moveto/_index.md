---
title: Worksheet.MoveTo
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Moves the sheet to another location in the spreadsheet
type: docs
url: /net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Moves the sheet to another location in the spreadsheet.

```csharp
public void MoveTo(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Destination sheet index. |

### Examples

```csharp
// Called: newWorksheet.MoveTo(i++);
[Test]
        public void Method_Int32_()
        {
            int i = 2;
            var names = new string[] { &quot;ws1&quot;, &quot;ws2&quot;, &quot;ws3&quot; };
            var workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44477.xlsx&quot;);
            var worksheet1 = workbook.Worksheets[0];
            var worksheet2 = workbook.Worksheets[1];

            foreach (var name in names)
            {
                Worksheet newWorksheet = workbook.Worksheets.Add(name);
                newWorksheet.MoveTo(i++);
                newWorksheet.Copy(worksheet1);
            }

            foreach (var name in names)
            {
                Worksheet newWorksheet = workbook.Worksheets.Add(name + &quot;_bis&quot;);
                newWorksheet.MoveTo(i++);
                newWorksheet.Copy(worksheet2);
            }
            Assert.AreEqual(&quot;Table15&quot;, workbook.Worksheets[6].ListObjects[1].DisplayName);
            workbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


