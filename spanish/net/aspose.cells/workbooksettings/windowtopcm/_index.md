---
title: "WorkbookSettings.WindowTopCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La distancia desde el borde superior del área cliente hasta el borde superior de la ventana en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidades de centímetro.

```csharp
public double WindowTopCM { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad WindowTopCM (posición desde la parte superior en centímetros)
            settings.WindowTopCM = 2.5;

            // Mostrar el valor actual de WindowTopCM
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // Guarda el libro de trabajo
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


