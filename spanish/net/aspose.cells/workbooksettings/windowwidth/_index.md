---
title: "WorkbookSettings.WindowWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "WorkbookSettings property. El ancho de la ventana en unidades de punto"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

El ancho de la ventana, en unidades de punto.

```csharp
public double WindowWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Establecer la propiedad WindowWidth
            settings.WindowWidth = 800;
            
            // Verificar el valor de WindowWidth
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // Guarda el libro de trabajo
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


