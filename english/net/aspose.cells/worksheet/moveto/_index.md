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
public void Worksheet_Method_MoveTo()
{
    int i = 2;
    var names = new string[] { "ws1", "ws2", "ws3" };
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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
        Worksheet newWorksheet = workbook.Worksheets.Add(name + "_bis");
        newWorksheet.MoveTo(i++);
        newWorksheet.Copy(worksheet2);
    }
    Assert.AreEqual("Table15", workbook.Worksheets[6].ListObjects[1].DisplayName);
    workbook.Save(Constants.destPath + "dest.xlsx");
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


