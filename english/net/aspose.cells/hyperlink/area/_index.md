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
// Called: if (link.Area.StartRow == 0 && link.Area.StartColumn == 0)
[Test]
        public void Property_Area()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "deu.epub");
            Assert.AreEqual("Calibre Kurzanleitung", workbook.Worksheets[0].Cells[0, 0].StringValue);
            Assert.AreEqual("Aufgabe 1: Organisieren", workbook.Worksheets[0].Cells[5, 0].StringValue);
            Assert.AreEqual(1, workbook.Worksheets[0].Cells[5, 0].GetStyle().IndentLevel);
            Assert.AreEqual(2, workbook.Worksheets[0].Cells[6, 0].GetStyle().IndentLevel); 
            HyperlinkCollection hyperlinks = workbook.Worksheets[0].Hyperlinks;
            string address1 = "",address2="";
            for (int i = 0; i < hyperlinks.Count; i++)
            {
                Hyperlink link = hyperlinks[i];
                if (link.Area.StartRow == 0 && link.Area.StartColumn == 0)
                {
                    address1 = link.Address;
                }
                else if (link.Area.StartRow == 21 && link.Area.StartColumn == 0)
                {
                    address2 = link.Address;
                    break;
                }
            }
            Assert.AreEqual("'Calibre Kurzanleitung'!A1", address1);
            Assert.AreEqual("'Wo Sie Hilfe bekommen'!A1", address2);
            Assert.AreEqual("'Aufgabe 6- Der eBook-Betrachter'!A1", workbook.Worksheets["Häufige Aufgaben"].Hyperlinks[5].Address);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


