---
title: ChartTextFrame.Characters
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame method. Returns a Characters object that represents a range of characters within the text
type: docs
url: /net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Returns a Characters object that represents a range of characters within the text.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the start of the character. |
| length | Int32 | The number of characters. |

### Return Value

Characters object.

### Examples

```csharp
// Called: Assert.AreEqual(11, chart.NSeries[0].Points[1].DataLabels.Characters(0, 1).Font.Size);
[Test]
        public void Method_Int32_()
        {
            Workbook lc_WorkBook = new Workbook(Constants.sourcePath + "CELLSJAVA-45431.xlsx");
            Chart chart = lc_WorkBook.Worksheets[0].Charts[0];

            Assert.AreEqual(11, chart.NSeries[0].Points[1].DataLabels.Characters(0, 1).Font.Size);
            lc_WorkBook.Save(Constants.destPath + "CELLSJAVA-45431.xlsx");
        }
```

### See Also

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


