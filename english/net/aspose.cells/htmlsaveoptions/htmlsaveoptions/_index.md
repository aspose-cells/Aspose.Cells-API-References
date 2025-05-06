---
title: HtmlSaveOptions.HtmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions constructor. Creates options for saving html file
type: docs
url: /net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

Creates options for saving html file.

```csharp
public HtmlSaveOptions()
```

### Examples

```csharp
// Called: var opts = new HtmlSaveOptions
[Test]
        public void HtmlSaveOptions_Constructor()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47501/&quot;;

            string savePath = CreateFolder(filePath);
            var wb = new Workbook(filePath + &quot;Excel2.xlsx&quot;);
            using (var stream = new MemoryStream(1))
            {
                var opts = new HtmlSaveOptions
                {
                    ExportActiveWorksheetOnly = true
                };
                wb.Save(stream, opts);
                byte[] arr = stream.ToArray();
                var html = Encoding.UTF8.GetString(arr);
                File.WriteAllText(savePath + &quot;out2.html&quot;, html);
            }

            var wb1 = new Workbook(filePath + &quot;Excel1.xlsx&quot;);
            using (var stream = new MemoryStream(1))
            {
                var opts = new HtmlSaveOptions
                {
                    ExportActiveWorksheetOnly = true
                };
                wb1.Save(stream, opts);
                byte[] arr = stream.ToArray();
                var html = Encoding.UTF8.GetString(arr);
                File.WriteAllText(savePath + &quot;out1.html&quot;, html);
            }
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving htm file.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Html or MHtml, otherwise the saved format will be set as Html automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


