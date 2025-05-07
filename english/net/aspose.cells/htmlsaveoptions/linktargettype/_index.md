---
title: HtmlSaveOptions.LinkTargetType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating the type of target attribute in a link. The default value is HtmlLinkTargetType.Parent
type: docs
url: /net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

Indicating the type of target attribute in `<a>` link. The default value is HtmlLinkTargetType.Parent.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
[Test]
        public void Property_LinkTargetType()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET44088/";

            string savePath = CreateFolder(filePath);
            Aspose.Cells.Workbook wb = new Workbook(filePath + "SampleFile.xlsx");
            wb.Save(savePath + "out.pdf");

            Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
            wb.Save(savePath + "out.html", htmlSaveOptions);

            wb = new Workbook(filePath + "a2.xlsx");
            wb.Save(savePath + "a2_out.html", htmlSaveOptions);
            wb.Save(savePath + "a2_out.pdf");

            wb = new Workbook(filePath + "a3.xlsx");
            wb.Save(savePath + "a3_out.html", htmlSaveOptions);
            wb.Save(savePath + "a3_out.pdf");
        }
```

### See Also

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


