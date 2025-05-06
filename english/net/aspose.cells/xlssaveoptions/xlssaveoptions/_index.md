---
title: XlsSaveOptions.XlsSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XlsSaveOptions constructor. Creates options for saving Excel 972003 xls file
type: docs
url: /net/aspose.cells/xlssaveoptions/xlssaveoptions/
---
## XlsSaveOptions() {#constructor}

Creates options for saving Excel 97-2003 xls file.

```csharp
public XlsSaveOptions()
```

### Examples

```csharp
// Called: XlsSaveOptions saveOptions = new XlsSaveOptions();
[Test]
        public void XlsSaveOptions_Constructor()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47308/&quot;;

            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            string htmlString1 = &quot;&lt;font style=\&quot;font-weight:normal; text-decoration:underline;color:red;\&quot;&gt;Red1&lt;/font&gt;&lt;font style=\&quot;font-weight:normal;text-decoration:underline;color:green;\&quot;&gt;Green1&lt;/font&gt;&quot;;
            var cell1 = ws.Cells[1, 1];
            cell1.HtmlString = htmlString1;

            //string htmlString2 = &quot;&lt;font style=\&quot;font-weight:normal; text-decoration:underline;color:red;\&quot;&gt;Red2&lt;/font&gt;&lt;font style=\&quot;font-weight:normal;text-decoration:underline;color:green;\&quot;&gt;Green2&lt;/font&gt;&quot;;
            var cell2 = ws.Cells[3, 1];
            cell2.HtmlString = htmlString1;
            var range2 = ws.Cells.CreateRange(3, 1, 5, 5);
            range2.Merge();
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            string savePath = CreateFolder(filePath);
            wb.Save(savePath + @&quot;out.xls&quot;, saveOptions);

            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            wb.Save(savePath + @&quot;out.htm&quot;, htmlSaveOptions);
        }
```

### See Also

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving Excel 97-2003 xls/xlt file.

```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be Excel97To2003 or Xlt, otherwise the saved format will be set as Excel97To2003 automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


