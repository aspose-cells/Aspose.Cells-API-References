---
title: Hyperlink.Area
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Gets the range of hyperlink
type: docs
url: /net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

Gets the range of hyperlink.

```csharp
public CellArea Area { get; }
```

### Examples

```csharp
// Called: if (link.Area.StartRow == 68 && link.Area.StartColumn == 0)
public void Hyperlink_Property_Area()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Bogtyven.epub");
    Assert.AreEqual("Indhold", workbook.Worksheets[0].Cells[0, 0].StringValue);
    Assert.AreEqual("1. Titel", workbook.Worksheets[0].Cells[2, 0].StringValue);
    Assert.AreEqual(1, workbook.Worksheets[0].Cells[3, 0].GetStyle().IndentLevel);
    HyperlinkCollection hyperlinks = workbook.Worksheets[0].Hyperlinks;
    string address = "";
    Assert.AreEqual(2, workbook.Worksheets[0].Cells[5, 0].GetStyle().IndentLevel);
    for (int i = 0; i < hyperlinks.Count; i++)
    {
        Hyperlink link = hyperlinks[i];
        if (link.Area.StartRow == 68 && link.Area.StartColumn == 0)
        {
            address = link.Address;
            break;
        }
    }
    Assert.AreEqual("'– Dødens dagbog- Pariserne'!A1", address);
    Assert.IsTrue(workbook.Worksheets["Prolog- En bjergkæde af murb..."].Cells[0, 0].GetStyle().Font.IsBold);

}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


