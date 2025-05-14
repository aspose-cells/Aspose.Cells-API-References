---
title: ExportObjectEvent.GetSource
second_title: Aspose.Cells for .NET API Reference
description: ExportObjectEvent method. Gets the object to be exported
type: docs
url: /net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Gets the object to be exported.

```csharp
public object GetSource()
```

### Return Value

the object to be exported.

### Examples

```csharp
// Called: Object source = e.GetSource();
public object ExportObjectEvent_Method_GetSource(ExportObjectEvent e)
        {
            Object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                return SaveImage(shape);
            }
            else if (source is ChartShape)
            {
                ChartShape chart = (ChartShape)source;
                return SaveChart(chart);
            }
            return null;
        }
```

### See Also

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


