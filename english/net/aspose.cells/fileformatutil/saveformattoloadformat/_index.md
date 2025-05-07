---
title: FileFormatUtil.SaveFormatToLoadFormat
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Converts a SaveFormat value to a LoadFormat value if possible
type: docs
url: /net/aspose.cells/fileformatutil/saveformattoloadformat/
---
## FileFormatUtil.SaveFormatToLoadFormat method

Converts a SaveFormat value to a LoadFormat value if possible.

```csharp
public static LoadFormat SaveFormatToLoadFormat(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format. |

### Return Value

The load format

### Examples

```csharp
// Called: LoadFormat ods = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Ods);
[Test]
        public static void Method_SaveFormat_()
        {
            //The annotated test code is currently not supported

            LoadFormat excel97To2003 = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Excel97To2003);
            Assert.AreEqual(LoadFormat.Excel97To2003, excel97To2003);

            LoadFormat xlsx = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsx);
            Assert.AreEqual(LoadFormat.Xlsx, xlsx);

            LoadFormat tsv = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Tsv);
            Assert.AreEqual(LoadFormat.Tsv, tsv);

            LoadFormat tabdelimited = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.TabDelimited);
            Assert.AreEqual(LoadFormat.TabDelimited, tabdelimited);

            LoadFormat ods = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Ods);
            Assert.AreEqual(LoadFormat.Ods, ods);

            LoadFormat spreadsheetml = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.SpreadsheetML);
            Assert.AreEqual(LoadFormat.SpreadsheetML, spreadsheetml);

            LoadFormat xlsb = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsb);
            Assert.AreEqual(LoadFormat.Xlsb, xlsb);

            LoadFormat numbers = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Numbers);
            Assert.AreEqual(LoadFormat.Numbers, numbers);
            
            //LoadFormat ots = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Ots);
            //Assert.AreEqual(LoadFormat.Ots, ots);

            //LoadFormat html = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Html);
            //Assert.AreEqual(LoadFormat.Html, html);

            //LoadFormat mhtml = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.MHtml);
            //Assert.AreEqual(LoadFormat.MHtml, mhtml);

            //LoadFormat xml = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xml);
            //Assert.AreEqual(LoadFormat.Xml, xml);

            //LoadFormat epub = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Epub);
            //Assert.AreEqual(LoadFormat.Epub, epub);

            //LoadFormat sxc = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Sxc);
            //Assert.AreEqual(LoadFormat.Sxc, sxc);

            //LoadFormat json = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Json);
            //Assert.AreEqual(LoadFormat.Json, json);

            //LoadFormat fods = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Csv);
            //Assert.AreEqual(LoadFormat.Fods, fods);

            //LoadFormat image = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Png);
            //Assert.AreEqual(LoadFormat.Image, image);

            //image = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Bmp);
            //Assert.AreEqual(LoadFormat.Image, image);

            //image = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Jpg);
            //Assert.AreEqual(LoadFormat.Image, image);

            //image = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Svg);
            //Assert.AreEqual(LoadFormat.Image, image);

        }
```

### See Also

* enum [LoadFormat](../../loadformat/)
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


