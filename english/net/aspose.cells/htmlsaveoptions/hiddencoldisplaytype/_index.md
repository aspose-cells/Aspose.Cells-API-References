---
title: HtmlSaveOptions.HiddenColDisplayType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Hidden columnthe width of this column is 0 in excelbefore save this into html format if HtmlHiddenColDisplayType is Removethe hidden column would not been output if the value is Hidden the column would been outputbut was hiddenthe default value is Hidden
type: docs
url: /net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Hidden column(the width of this column is 0) in excel,before save this into html format, if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output, if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden"

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Examples

```csharp
// Called: HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
public void HtmlSaveOptions_Property_HiddenColDisplayType()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47490/";

    var options = new HtmlSaveOptions
    {
        ExportImagesAsBase64 = true,
        ExportSingleTab = true,
        ExportHiddenWorksheet = false,
        ExportGridLines = true,
        HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
        HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
    };
    Workbook wb = null;
    string savePath = CreateFolder(filePath);
    wb = new Workbook(filePath + "hidden_AllObjectsHiddenFromWorkbookPr.xlsx");
    wb.Save(savePath + "out1.html", options);
    wb = new Workbook(filePath + "hidden_GroupedObjectsMarkedAsHidden.xlsx");
    wb.Save(savePath + "out2.html", options);
    wb = new Workbook(filePath + "hidden_TableWithHiddenSlicer.xlsx");
    wb.Save(savePath + "out3.html", options);
}
```

### See Also

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


