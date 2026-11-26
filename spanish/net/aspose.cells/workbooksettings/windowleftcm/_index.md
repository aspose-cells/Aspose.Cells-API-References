---
title: "WorkbookSettings.WindowLeftCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de centímetros"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowleftcm/
---
## WorkbookSettings.WindowLeftCM property

La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de centímetro.

```csharp
public double WindowLeftCM { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftCMDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad WindowLeftCM (distancia desde el borde izquierdo de la pantalla en centímetros)
            settings.WindowLeftCM = 2.54; // 1 inch = 2.54 cm

            // Verificar la configuración imprimiéndola
            Console.WriteLine("WindowLeftCM: " + settings.WindowLeftCM);

            // Guarda el libro de trabajo
            workbook.Save("WindowLeftCMDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


