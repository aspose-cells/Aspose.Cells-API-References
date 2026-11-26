---
title: "WorkbookSettings.WindowWidthCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. El ancho de la ventana en unidades de centímetro"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowwidthcm/
---
## WorkbookSettings.WindowWidthCM property

El ancho de la ventana, en unidades de centímetro.

```csharp
public double WindowWidthCM { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthCMDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Establecer la propiedad WindowWidthCM (20.32 cm = ~8 pulgadas)
            settings.WindowWidthCM = 20.32;
            
            // Verificar la configuración imprimiéndola
            Console.WriteLine("Window Width in Centimeters: " + settings.WindowWidthCM);
            
            // Guarda el libro de trabajo
            workbook.Save("WindowWidthCMDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


