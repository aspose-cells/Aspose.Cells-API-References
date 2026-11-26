---
title: "WorkbookSettings.WindowLeft"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana en unidades de punto"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana, en unidades de punto.

```csharp
public double WindowLeft { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad WindowLeft para posicionar la ventana a 100 píxeles desde la izquierda
            settings.WindowLeft = 100;

            // Establecer otras propiedades de la ventana para la demostración
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // Agregar datos de muestra a la hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // Guarda el libro de trabajo
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


