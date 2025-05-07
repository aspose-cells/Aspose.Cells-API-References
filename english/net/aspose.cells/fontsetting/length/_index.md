---
title: FontSetting.Length
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Gets the length of the characters
type: docs
url: /net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Gets the length of the characters.

```csharp
public int Length { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(8, fs[1].Length);
[Test]
        public void Property_Length()
        {
            Workbook wb = new Workbook(Constants.sourcePath + @"Numbers13\CELLSNET48352.numbers");
            Cells cells = wb.Worksheets[0].Cells;
            Cell d3 = cells["D3"];
            Assert.IsTrue(d3.IsRichText());
            FontSetting[] fs = d3.GetCharacters();
            Assert.AreEqual(3, fs.Length);
            Assert.AreEqual(2, fs[1].StartIndex);
            Assert.AreEqual(8, fs[1].Length);
            AssertHelper.AreEqual(System.Drawing.Color.Red, fs[1].Font.Color);
            Assert.AreEqual("sdfsdfsdfsdfsdf", d3.StringValue);
            Util.ReSave(wb, SaveFormat.Xlsx);
            //wb.Save(Constants.destPath + "CELLSNET48125.xlsx");
        }
```

### See Also

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


