---
title: ChartFrame.IsAutomaticSize
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Indicates whether the chart frame is automatic sized
type: docs
url: /net/aspose.cells.charts/chartframe/isautomaticsize/
---
## ChartFrame.IsAutomaticSize property

Indicates whether the chart frame is automatic sized.

```csharp
public virtual bool IsAutomaticSize { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].Legend.IsAutomaticSize, false);
[Test]
        public void Property_IsAutomaticSize()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "UnmodifiedInput.xls");
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].Legend.IsAutomaticSize, false);
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


