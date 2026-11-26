---
title: "WorkbookSettings.WindowWidthInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. El ancho de la ventana en unidades de pulgada"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

El ancho de la ventana, en unidades de pulgada.

```csharp
public double WindowWidthInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer el ancho de la ventana en pulgadas
            settings.WindowWidthInch = 10.5;

            // Mostrar el ancho de la ventana en pulgadas
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // Guarda el libro de trabajo
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


