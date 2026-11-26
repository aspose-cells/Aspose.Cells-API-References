---
title: "WorkbookSettings.WindowHeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La altura de la ventana en unidades de pulgada"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

La altura de la ventana, en unidades de pulgada.

```csharp
public double WindowHeightInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer la altura de la ventana en pulgadas
            settings.WindowHeightInch = 5.5;

            // Mostrar la altura de la ventana en pulgadas
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // Guarda el libro de trabajo
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


