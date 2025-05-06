---
title: HtmlSaveOptions.CellNameAttribute
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Specifies the attribute that indicates the CellName to be written. e.g. If the value is id then for cell A1 the output will betd idA1. The default value is null
type: docs
url: /net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.

```csharp
public string CellNameAttribute { get; set; }
```

### Examples

```csharp
// Called: saveOptions.CellNameAttribute = &amp;quot;id&amp;quot;;
[Test]
        public void Property_CellNameAttribute()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-46180.xlsx&quot;);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = &quot;id&quot;;
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;
            workbook.Save(_destFilesPath + &quot;CELLSJAVA-46180.html&quot;, saveOptions);
            string text = File.ReadAllText(_destFilesPath + &quot;CELLSJAVA-46180.html&quot;);
            string pattern = @&quot;&lt;td\s+id=&apos;A23&apos;\s+[^&gt;]*style=&apos;[^&apos;]*background:*#FFFFFF;[^&apos;]*&apos;[^&gt;]*&gt;&quot;; 
            Assert.IsTrue(Regex.IsMatch(text, pattern));
            pattern = @&quot;&lt;td\s+id=&apos;B27&apos;\s+[^&gt;]*style=&apos;[^&apos;]*background:*#FFFFFF;[^&apos;]*&apos;[^&gt;]*&gt;&quot;;
            Assert.IsTrue(Regex.IsMatch(text, pattern));
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


