---
title: HtmlLoadOptions.HasFormula
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether the text is formula if it starts with 
type: docs
url: /net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Indicates whether the text is formula if it starts with "=".

```csharp
public bool HasFormula { get; set; }
```

### Examples

```csharp
// Called: loadOptions.HasFormula = false;
[Test]
        public void Property_HasFormula()
        {
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.ConvertNumericData = true;
            loadOptions.ConvertDateTimeData = false;
            loadOptions.HasFormula = false;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.SupportDivTag = true;

            loadOptions.AutoFitColsAndRows = true;

            //loadOptions.Encoding = System.Text.Encoding.GetEncoding(&quot;ISO-8859-1&quot;);


            // Create a Workbook object and opening the file from its path
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSNET-49031.html&quot;, loadOptions);

            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(&quot;Daytime &quot;, cells[&quot;A1&quot;].StringValue);
            Assert.AreEqual(&quot;After-Hours&quot;, cells[&quot;B1&quot;].StringValue);
            Assert.AreEqual(&quot;Backup&quot;, cells[&quot;C1&quot;].StringValue);

            Assert.AreEqual(&quot;Employee Away Information&quot;, cells[&quot;A11&quot;].StringValue);

            // Save the MHT file
            wb.Save(_destFilesPath + &quot;CELLSNET-49031.xlsx&quot;);
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


