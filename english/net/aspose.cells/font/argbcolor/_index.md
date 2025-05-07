---
title: Font.ArgbColor
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the color with a 32bit ARGB value
type: docs
url: /net/aspose.cells/font/argbcolor/
---
## Font.ArgbColor property

Gets and sets the color with a 32-bit ARGB value.

```csharp
public int ArgbColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0xFFFF0000, cell.GetDisplayStyle().Font.ArgbColor & 0xFFFFFFFF);
[Test]
        public void Property_ArgbColor()
        {
            string sourcePath = Constants.sourcePath + "CELLSNET-49610/";
            Workbook wb = new Workbook(sourcePath + "Template.xlsx");

            wb.ImportXml(sourcePath + "xml.xml", "Sheet1", 0, 0);

            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                ms.Position = 0;

                Workbook reloadWb = new Workbook(ms);
                Worksheet sheet = reloadWb.Worksheets[0];
                Assert.AreEqual(148, sheet.ListObjects[0].EndRow + 1);

                Cells cells = sheet.Cells;
                Cell cell = cells["A148"];
                Assert.AreEqual("AGR/SB/WATERGANG3078", cell.DisplayStringValue);
                Assert.AreEqual(0xFFFFFF00, cell.GetDisplayStyle().ForegroundArgbColor & 0xFFFFFFFF);

                cell = cells["J148"];
                Assert.AreEqual("Bellville", cell.DisplayStringValue);
                Assert.AreEqual(0xFF4472C4, cell.GetDisplayStyle().ForegroundArgbColor & 0xFFFFFFFF);

                cell = cells["F148"];
                Assert.AreEqual("29 January 2021", cell.DisplayStringValue);
                Assert.AreEqual(0xFFFF0000, cell.GetDisplayStyle().Font.ArgbColor & 0xFFFFFFFF);


                //TODO:
                //Assert.AreEqual("04228958007", cells["C148"].DisplayStringValue);
                //Assert.AreEqual("Domestic Low 01", cells["D148"].DisplayStringValue);
                //Assert.AreEqual("Cape Town", cells["H148"].DisplayStringValue);
                //Assert.AreEqual("NP_TEST", cells["G148"].DisplayStringValue);

                //Assert.IsTrue(string.IsNullOrEmpty(cells["C25"].DisplayStringValue));
                //Assert.IsTrue(string.IsNullOrEmpty(cells["D25"].DisplayStringValue));

                //Assert.IsTrue(string.IsNullOrEmpty(cells["H39"].DisplayStringValue));
                //Assert.IsTrue(string.IsNullOrEmpty(cells["I39"].DisplayStringValue));


            }

        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


