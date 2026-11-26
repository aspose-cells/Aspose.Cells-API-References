---
title: "PageSetup.Orientation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa la orientación de impresión de la página"
type: docs
url: /es/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Representa la orientación de impresión de la página.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la orientación de la página a Horizontal
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // Agregar algunos datos de ejemplo para demostrar el efecto
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


