---
title: "WorkbookSettings.WindowTopInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. La distancia desde el borde superior del área cliente hasta el borde superior de la ventana en unidades de pulgada"
type: docs
url: /es/net/aspose.cells/workbooksettings/windowtopinch/
---
## WorkbookSettings.WindowTopInch property

La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidades de pulgada.

```csharp
public double WindowTopInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Establecer la propiedad WindowTopInch para posicionar la ventana a 2 pulgadas desde la parte superior
            settings.WindowTopInch = 2.0;

            // Verificar la configuración imprimiéndola
            Console.WriteLine("Window top position (inches): " + settings.WindowTopInch);

            // Guarda el libro de trabajo
            workbook.Save("WindowTopInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


