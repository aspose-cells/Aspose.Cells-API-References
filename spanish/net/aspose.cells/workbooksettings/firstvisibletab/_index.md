---
title: "WorkbookSettings.FirstVisibleTab"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece la primera pestaña de hoja de cálculo visible"
type: docs
url: /es/net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

Obtiene o establece la primera pestaña de hoja visible.

```csharp
public int FirstVisibleTab { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFirstVisibleTabDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Establezca el índice de la primera pestaña visible (basado en 0)
            workbook.Settings.FirstVisibleTab = 1;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Verifique la configuración
            Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


