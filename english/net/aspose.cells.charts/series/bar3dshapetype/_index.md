---
title: Series.Bar3DShapeType
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets the 3D shape type used with the 3D bar or column chart
type: docs
url: /net/aspose.cells.charts/series/bar3dshapetype/
---
## Series.Bar3DShapeType property

Gets or sets the 3D shape type used with the 3-D bar or column chart.

```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.ConeToMax;
[Test]
        public void Property_Bar3DShapeType()
        {
            Workbook workbook = new Workbook();
            workbook = TestCylinder.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.ConeToMax;

            checkBar3DShapeType_ConeToMax(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkBar3DShapeType_ConeToMax(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkBar3DShapeType_ConeToMax(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


