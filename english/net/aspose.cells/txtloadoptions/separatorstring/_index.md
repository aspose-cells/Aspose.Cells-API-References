---
title: TxtLoadOptions.SeparatorString
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Gets and sets a string value as separator
type: docs
url: /net/aspose.cells/txtloadoptions/separatorstring/
---
## TxtLoadOptions.SeparatorString property

Gets and sets a string value as separator.

```csharp
public string SeparatorString { get; set; }
```

### Examples

```csharp
// Called: loadOptions.SeparatorString = &amp;quot;,&amp;quot;;
[Test]
        public void Property_SeparatorString()
        {
            string FileName = Constants.sourcePath + &quot;TestWorkbook\\Book1.xls&quot;;
            Workbook workbook = new Workbook(FileName);
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            saveOptions.SeparatorString = &quot;,&quot;;
            workbook.Save(Constants.destPath + &quot;testSave.CSV&quot;, saveOptions);

            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = &quot;,&quot;;
            workbook = new Workbook(Constants.destPath + &quot;testSave.CSV&quot;, loadOptions);
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(&quot;Tabelle1&quot;, cells[1, 1].StringValue);
            Assert.AreEqual(3, cells[3, 2].IntValue);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


