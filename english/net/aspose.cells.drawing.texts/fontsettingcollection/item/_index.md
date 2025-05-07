---
title: FontSettingCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: FontSettingCollection property. Gets the FontSetting by the index
type: docs
url: /net/aspose.cells.drawing.texts/fontsettingcollection/item/
---
## FontSettingCollection indexer

Gets the [`FontSetting`](../../../aspose.cells/fontsetting/) by the index.

```csharp
public FontSetting this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: Assert.AreEqual(copyWorkbook.Worksheets[0].Charts[0].Shapes[0].TextBody[1].Font.Name, "Gill Sans MT");
[Test]
        public void Property_Int32_()
        {
            var modelWorkbook = new Workbook(Constants.sourcePath + "CELLSNET44566_1.xlsx");
            Workbook copyWorkbook = new Workbook();
            copyWorkbook.Copy(modelWorkbook);
            Assert.AreEqual(copyWorkbook.Worksheets[0].Shapes[0].TextBody[1].Font.Name, "Segoe Marker");
            copyWorkbook.Save(Constants.destPath + @"CELLSNET44566_1.xlsx");
            modelWorkbook = new Workbook(Constants.sourcePath + "CELLSNET44566_2.xlsx");
            copyWorkbook = new Workbook();
            copyWorkbook.Copy(modelWorkbook);
            Assert.AreEqual(copyWorkbook.Worksheets[0].Charts[0].Shapes[0].TextBody[1].Font.Name, "Gill Sans MT");
           AssertHelper.AreEqual(copyWorkbook.Worksheets[0].Charts[0].ChartArea.Area.ForegroundColor,System.Drawing.Color.White);
            Util.ReSave(copyWorkbook, SaveFormat.Xlsx);
            //copyWorkbook.Save(Constants.destPath + @"CELLSNET44566_2.xlsx"); 
        }
```

### See Also

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


