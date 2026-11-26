---
title: "WorkbookSettings.WindowHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La altura de la ventana en unidades de punto"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

La altura de la ventana, en unidades de punto.

```csharp
public double WindowHeight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Establezca la propiedad WindowHeight
            settings.WindowHeight = 600;
            
            // Verifique el valor de WindowHeight
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
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


