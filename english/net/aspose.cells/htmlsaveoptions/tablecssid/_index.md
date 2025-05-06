---
title: HtmlSaveOptions.TableCssId
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets and sets the prefix of the type css name such as trcoltd and so on they are contained in the table element which has the specific TableCssId attribute. The default value is 
type: docs
url: /net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```csharp
public string TableCssId { get; set; }
```

### Examples

```csharp
// Called: saveOptions.TableCssId = &amp;quot;asdf&amp;quot;;
[Test]
        public void Property_TableCssId()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42465/&quot;;
            Workbook workbook = new Workbook(filePath + &quot;input.xlsx&quot;);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.ExportHiddenWorksheet = false;
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.CellCssPrefix = &quot;prefix123&quot;;
            saveOptions.TableCssId = &quot;asdf&quot;;
            workbook.Save(CreateFolder(filePath) + &quot;out.html&quot;, saveOptions);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


