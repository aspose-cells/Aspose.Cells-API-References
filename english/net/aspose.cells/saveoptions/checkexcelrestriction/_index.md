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
            string str = Repeat("x",32767) + " Testing if it works or not";
            cells["A1"].PutValue(str);
            Assert.AreEqual(str, cells["A1"].StringValue);
          

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            workbook.Save(Constants.destPath + "CellsJava46191.xlsx", saveOptions);

            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            workbook = new Workbook(Constants.destPath + "CellsJava46191.xlsx", loadOptions);
            Assert.AreEqual(str, workbook.Worksheets[0].Cells["A1"].StringValue);
            Assert.IsTrue(workbook.Worksheets[0].Cells["A1"].StringValue.Length > short.MaxValue);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


