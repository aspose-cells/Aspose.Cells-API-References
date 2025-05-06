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
// Called: options.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
[Test]
        public void Property_HiddenColDisplayType()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41562/&quot;;
            Workbook wb = new Workbook(filePath + &quot;Test.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            options.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            wb.Save(CreateFolder(filePath) + &quot;out.html&quot;, options);
        }
```

### See Also

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


