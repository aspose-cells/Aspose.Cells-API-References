---
title: "WorkbookSettings.WindowLeftInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de pulgada"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowleftinch/
---
## WorkbookSettings.WindowLeftInch property

La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de pulgada.

```csharp
public double WindowLeftInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad WindowLeftInch
            settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen

            // Agregar algunos datos de ejemplo para demostrar que el libro de trabajo funciona
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");

            // Guarda el libro de trabajo
            workbook.Save("WindowLeftInchDemo.xlsx");

            Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


