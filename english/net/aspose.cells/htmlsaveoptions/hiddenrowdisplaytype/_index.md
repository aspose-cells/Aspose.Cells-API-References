---
title: HtmlSaveOptions.HiddenRowDisplayType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Hidden rowthe height of this row is 0 in excelbefore save this into html format if HtmlHiddenRowDisplayType is Removethe hidden row would not been output if the value is Hidden the row would been outputbut was hiddenthe default value is Hidden
type: docs
url: /net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Hidden row(the height of this row is 0) in excel,before save this into html format, if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output, if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Examples

```csharp
// Called: options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
public void HtmlSaveOptions_Property_HiddenRowDisplayType()
{
          
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.DisableDownlevelRevealedComments = true;
    options.ExcludeUnusedStyles = true;
    options.IsExportComments = false;
    options.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
    options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
    options.ExportBogusRowData = true;
    options.ExportFrameScriptsAndProperties = false;
    options.WidthScalable = false;
    options.ExportHeadings = true;
    workbook.Save(Constants.destPath + "example.html", options);
    workbook = new Workbook(Constants.destPath + "example.html");
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.AreEqual("6", cells["A7"].StringValue);
    Assert.IsTrue(cells.IsRowHidden(6));
}
```

### See Also

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


