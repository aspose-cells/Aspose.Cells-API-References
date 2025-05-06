---
title: SaveOptions.CheckExcelRestriction
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K it will be truncated
type: docs
url: /net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Examples

```csharp
// Called: saveOptions.CheckExcelRestriction = false;
[Test]
        public void Property_CheckExcelRestriction()
        {
            Workbook wb = new Workbook();
            Workbook workbook = new Workbook();
            workbook.Settings.CheckExcelRestriction = false;

            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            string str = Repeat(&quot;x&quot;,32767) + &quot; Testing if it works or not&quot;;
            cells[&quot;A1&quot;].PutValue(str);
            Assert.AreEqual(str, cells[&quot;A1&quot;].StringValue);
          

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            workbook.Save(Constants.destPath + &quot;CellsJava46191.xlsx&quot;, saveOptions);

            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            workbook = new Workbook(Constants.destPath + &quot;CellsJava46191.xlsx&quot;, loadOptions);
            Assert.AreEqual(str, workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
            Assert.IsTrue(workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue.Length &gt; short.MaxValue);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


