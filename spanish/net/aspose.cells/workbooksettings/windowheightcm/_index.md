---
title: "WorkbookSettings.WindowHeightCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La altura de la ventana en unidades de centímetro"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

La altura de la ventana, en unidades de centímetro.

```csharp
public double WindowHeightCM { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad WindowHeightCM
            settings.WindowHeightCM = 15.5;

            // Mostrar el valor establecido
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

            // Guarda el libro de trabajo
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


