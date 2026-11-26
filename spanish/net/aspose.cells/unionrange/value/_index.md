---
title: "UnionRange.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene y establece los valores del rango"
type: docs
url: /es/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Obtiene y establece los valores del rango.

```csharp
public object Value { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un rango de unión usando la API correcta
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // Establece el valor para todo el rango de unión
            unionRange.Value = "Test Value";
            
            // Cree y aplique estilo
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Guarda el libro de trabajo
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


