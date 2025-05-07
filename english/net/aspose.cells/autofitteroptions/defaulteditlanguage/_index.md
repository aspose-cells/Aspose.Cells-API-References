---
title: AutoFitterOptions.DefaultEditLanguage
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets or sets default edit language
type: docs
url: /net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Gets or sets default edit language.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Remarks

It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.

### Examples

```csharp
// Called: fitterOptions.DefaultEditLanguage = DefaultEditLanguage.Auto;
[Test]
        public void Property_DefaultEditLanguage()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            Style style3 = workbook.CreateStyle();
            style3.Font.Name = "宋体";
            style3.Font.Size = 12;
            style3.IsTextWrapped = true;
            var sheet = workbook.Worksheets.Add("test");
            sheet.Cells.SetColumnWidthPixel(1, 200); //setwidth
                                                     //Spaces in different positions will get different result,40,60
                                                     //but if open the excel,they are the same
            string str1 = "测试数据的换行问题12121212121212 测试数据换行";
            string str2 = "测试数据的换行问题 12121212121212测试数据换行";
            Cells cells = sheet.Cells;
            cells[1, 1].PutValue(str1);
            cells[1, 1].SetStyle(style3);
            var h1 = cells[1, 1].GetHeightOfValue();
            Assert.AreEqual(57, h1);
            cells[2, 1].PutValue(str2);
            cells[2, 1].SetStyle(style3);
            var h2 = cells[2, 1].GetHeightOfValue();
            Assert.AreEqual(57, h2);
            AutoFitterOptions fitterOptions = new AutoFitterOptions();
            fitterOptions.DefaultEditLanguage = DefaultEditLanguage.Auto;
            sheet.AutoFitRows(fitterOptions);
            Assert.AreEqual(57, cells.GetRowHeightPixel(1));
            Assert.AreEqual(57, cells.GetRowHeightPixel(2));
            workbook.Save(Constants.destPath + "CellsNet47861.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


