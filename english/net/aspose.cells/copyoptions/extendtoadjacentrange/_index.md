---
title: CopyOptions.ExtendToAdjacentRange
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. Indicates whether extend ranges when copying the range to adjacent range
type: docs
url: /net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Indicates whether extend ranges when copying the range to adjacent range.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Remarks

If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

### Examples

```csharp
// Called: co.ExtendToAdjacentRange = true;
public void CopyOptions_Property_ExtendToAdjacentRange()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");

    Worksheet ws = wb.Worksheets["Sheet1"];

    HyperlinkCollection hyps = ws.Hyperlinks;

    int cnt1 = hyps.Count;

    CopyOptions co = new CopyOptions();
    co.ExtendToAdjacentRange = true;

    Cells cells = ws.Cells;
    cells.CopyRows(cells, 0, 1, 1, co);

    int cnt2 = hyps.Count;
   Assert.AreEqual(1,cnt2);
}
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


