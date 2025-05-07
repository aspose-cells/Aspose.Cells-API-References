---
title: DataLabels.IsTextWrapped
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets a value indicating whether the text is wrapped
type: docs
url: /net/aspose.cells.charts/datalabels/istextwrapped/
---
## DataLabels.IsTextWrapped property

Gets or sets a value indicating whether the text is wrapped.

```csharp
public override bool IsTextWrapped { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(outWorksheets[0].Charts[0].NSeries[0].DataLabels.IsTextWrapped);
[Test]
        public void Property_IsTextWrapped()
        {
            Workbook outWorkbook = new Workbook();
            WorksheetCollection outWorksheets = outWorkbook.Worksheets;
            outWorksheets.RemoveAt(0);
            Workbook slideWorkbook = new Workbook(Constants.sourcePath + "CellsJava41390.xlsx");
            WorksheetCollection slideWorksheets = slideWorkbook.Worksheets;
            outWorksheets.Add("data");
            outWorksheets[0].Copy(slideWorksheets[0]);
            Assert.IsFalse(outWorksheets[0].Charts[0].NSeries[0].DataLabels.IsTextWrapped);
            outWorkbook.Save(Constants.destPath + "CellsJava41390.xlsx");
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


