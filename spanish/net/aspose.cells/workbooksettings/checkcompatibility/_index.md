---
title: "WorkbookSettings.CheckCompatibility"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si se debe comprobar la compatibilidad con versiones anteriores al guardar el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/checkcompatibility/
---
## WorkbookSettings.CheckCompatibility property

Indica si se verifica la compatibilidad con versiones anteriores al guardar el libro.

```csharp
public bool CheckCompatibility { get; set; }
```

### Observaciones

El valor predeterminado es true. Solo para archivos Excel97-2003 xls o xlt.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCompatibilityDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer CheckCompatibility a true y guardar
            workbook.Settings.CheckCompatibility = true;
            workbook.Save("CheckCompatibilityDemo_true.xlsx");
            
            // Recargar y verificar
            workbook = new Workbook("CheckCompatibilityDemo_true.xlsx");
            Console.WriteLine("CheckCompatibility (true): " + workbook.Settings.CheckCompatibility);
            
            // Establecer CheckCompatibility a false y guardar
            workbook.Settings.CheckCompatibility = false;
            workbook.Save("CheckCompatibilityDemo_false.xlsx");
            
            // Recargar y verificar
            workbook = new Workbook("CheckCompatibilityDemo_false.xlsx");
            Console.WriteLine("CheckCompatibility (false): " + workbook.Settings.CheckCompatibility);
            
            // Demostrar operaciones de color
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color customColor = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
            Console.WriteLine("Matching color R value: " + customColor.R);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


