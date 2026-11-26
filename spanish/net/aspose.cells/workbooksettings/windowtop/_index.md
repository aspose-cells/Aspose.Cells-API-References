---
title: "WorkbookSettings.WindowTop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La distancia desde el borde superior del área cliente hasta el borde superior de la ventana en unidades de punto"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowtop/
---
## WorkbookSettings.WindowTop property

La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidades de punto.

```csharp
public double WindowTop { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad WindowTop para posicionar la ventana a 100 píxeles desde la parte superior
            settings.WindowTop = 100;
            
            // Verificar el valor de WindowTop
            Console.WriteLine("Window top position set to: " + settings.WindowTop);

            // Guarda el libro de trabajo
            workbook.Save("WindowTopDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


