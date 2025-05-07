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
// Called: HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
[Test]
        public void Property_HiddenColDisplayType()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSNET-49825.xls");
            var opt = new Aspose.Cells.HtmlSaveOptions
            {
                ExportHiddenWorksheet = false,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
                ExportImagesAsBase64 = true
            };

            Stopwatch watch = new Stopwatch();
            watch.Start();
            wb.Save(_destFilesPath + "CELLSNET-49825.html", opt);
            watch.Stop();
            Assert.IsTrue(watch.ElapsedMilliseconds < 5000);
        }
```

### See Also

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


