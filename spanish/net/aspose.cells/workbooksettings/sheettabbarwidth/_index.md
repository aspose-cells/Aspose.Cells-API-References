---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Ancho de la barra de pestañas de la hoja de cálculo en 1/1000 del ancho de la ventana"
type: docs
url: /es/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Ancho de la barra de pestañas de la hoja de cálculo (en 1/1000 del ancho de la ventana).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer la propiedad SheetTabBarWidth
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // Obtener y mostrar el valor de SheetTabBarWidth
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


