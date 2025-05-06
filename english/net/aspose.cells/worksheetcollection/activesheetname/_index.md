---
title: WorksheetCollection.ActiveSheetName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents the name of active worksheet when the spreadsheet is opened
type: docs
url: /net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Represents the name of active worksheet when the spreadsheet is opened.

```csharp
public string ActiveSheetName { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets.ActiveSheetName = &amp;quot;Sheet1&amp;quot;;
[Test]
        public void Property_ActiveSheetName()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSNET-49624.xlsx&quot;);
            wb.Worksheets.ActiveSheetName = &quot;Sheet1&quot;;
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            wb.Save(_destFilesPath + &quot;CELLSNET-49624.html&quot;, saveOptions);
            string text = File.ReadAllText(_destFilesPath + &quot;CELLSNET-49624.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;overflow:hidden;&apos;&gt;西吉县党家岔湿地保护区管理处&lt;/td&gt;&quot;) != -1);
            Assert.IsTrue(text.IndexOf(&quot;（一）加强&lt;span style=&apos;display:none&apos;&quot;) != -1);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


