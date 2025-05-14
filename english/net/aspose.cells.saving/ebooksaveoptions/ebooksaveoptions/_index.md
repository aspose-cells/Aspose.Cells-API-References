---
title: EbookSaveOptions.EbookSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: EbookSaveOptions constructor. Creates options for saving ebook file
type: docs
url: /net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

Creates options for saving ebook file.

```csharp
public EbookSaveOptions()
```

### Examples

```csharp
// Called: EbookSaveOptions saveOptions = new EbookSaveOptions();
public void EbookSaveOptions_Constructor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "EpubTest.xlsx");
    EbookSaveOptions saveOptions = new EbookSaveOptions();
    workbook.Save(Constants.destPath + "epubtest.epub", saveOptions);
    Workbook wb2 = new Workbook(Constants.destPath + "epubtest.epub");
    Worksheet ws = wb2.Worksheets["Growing Flowers"];
    string link1 = null, link2 = null;
    for (int i = 0; i < ws.Hyperlinks.Count; i++)
    {
        Hyperlink link = ws.Hyperlinks[i];
        if (link.Area.StartRow == 0 && link.Area.StartColumn == 0)
        {
            link1 = link.Address;
        }
        else if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
        {
            link2 = link.Address;
            break;
        }
    }
    Assert.AreEqual("'Introduction'!A1", link1);
    Assert.AreEqual("'Use'!A1", link2);
    ws = wb2.Worksheets["Introduction"];
    Assert.AreEqual(1, ws.Pictures.Count);
    Assert.IsTrue(ws.Pictures[0].Data.Length > 0);
    Assert.AreEqual("'Snowdrop'!A1", wb2.Worksheets["Use"].Hyperlinks[0].Address);
    ws = wb2.Worksheets["Pruning"];
    Assert.IsTrue(ws.Cells["A3"].GetCharacters()[0].Font.IsBold);
}
```

### See Also

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving ebook file.

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Epub or Azw3. |

### See Also

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


