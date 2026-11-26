---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookSettings. Establece el tipo de orientación de impresión para todo el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Establece el tipo de orientación de impresión para todo el libro de trabajo.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | El tipo de orientación de página |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            
            // Establecer la orientación de página a Retrato para todas las hojas de cálculo
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // Verificar que la orientación esté configurada correctamente
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### Ver también

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


