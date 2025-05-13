---
title: PasteOptions.Transpose
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. True to transpose rows and columns when the range is pasted. The default value is False
type: docs
url: /net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

True to transpose rows and columns when the range is pasted. The default value is False.

```csharp
public bool Transpose { get; set; }
```

### Examples

```csharp
// Called: pstoption.Transpose = (true);
public void PasteOptions_Property_Transpose()
{
    Workbook workbook = new Workbook();
    Worksheet ws = workbook.Worksheets[0];
    Cells cells = ws.Cells;

    Style style = workbook.CreateStyle();
    style.ForegroundColor = (Color.Yellow);
    style.Pattern = (BackgroundType.Solid);

    PasteOptions pstoption = new PasteOptions();
    pstoption.PasteType = (PasteType.Formats);
    pstoption.Transpose = (true);

    Aspose.Cells.Range range = cells.CreateRange(1, 1, 1, 4);
    range.SetStyle(style);

    Aspose.Cells.Range range2 = cells.CreateRange(6, 1, 9, 1);
    range2.Copy(range, pstoption);
    Assert.AreEqual(range2[0, 0].GetStyle().Pattern, BackgroundType.Solid);

       
}
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


