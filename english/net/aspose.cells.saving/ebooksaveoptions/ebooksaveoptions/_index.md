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
[Test]
        public void EbookSaveOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;EpubTest.xlsx&quot;);
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            workbook.Save(Constants.destPath + &quot;epubtest.epub&quot;, saveOptions);
            Workbook wb2 = new Workbook(Constants.destPath + &quot;epubtest.epub&quot;);
            Worksheet ws = wb2.Worksheets[&quot;Growing Flowers&quot;];
            string link1 = null, link2 = null;
            for (int i = 0; i &lt; ws.Hyperlinks.Count; i++)
            {
                Hyperlink link = ws.Hyperlinks[i];
                if (link.Area.StartRow == 0 &amp;&amp; link.Area.StartColumn == 0)
                {
                    link1 = link.Address;
                }
                else if (link.Area.StartRow == 3 &amp;&amp; link.Area.StartColumn == 0)
                {
                    link2 = link.Address;
                    break;
                }
            }
            Assert.AreEqual(&quot;&apos;Introduction&apos;!A1&quot;, link1);
            Assert.AreEqual(&quot;&apos;Use&apos;!A1&quot;, link2);
            ws = wb2.Worksheets[&quot;Introduction&quot;];
            Assert.AreEqual(1, ws.Pictures.Count);
            Assert.IsTrue(ws.Pictures[0].Data.Length &gt; 0);
            Assert.AreEqual(&quot;&apos;Snowdrop&apos;!A1&quot;, wb2.Worksheets[&quot;Use&quot;].Hyperlinks[0].Address);
            ws = wb2.Worksheets[&quot;Pruning&quot;];
            Assert.IsTrue(ws.Cells[&quot;A3&quot;].GetCharacters()[0].Font.IsBold);
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


