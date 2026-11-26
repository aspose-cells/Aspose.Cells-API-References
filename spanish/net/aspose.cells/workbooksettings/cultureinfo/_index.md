---
title: "WorkbookSettings.CultureInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece la información de cultura del sistema"
type: docs
url: /es/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Obtiene o establece la información de cultura del sistema.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Observaciones

Devuelve null si la información de cultura no está establecida y [`Region`](../region/) no está establecida.

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            
            // Establecer la región a Francia para demostrar los cambios de CultureInfo
            wb.Settings.Region = CountryCode.France;
            
            // Obtener el separador de grupos de la cultura francesa
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // Crear un estilo con formato personalizado y mostrar el formato ajustado a la cultura
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // Demostrar el formato de números con la cultura francesa
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells["A1"];
            cell.PutValue(123456.78);
            cell.SetStyle(style);
            style.Custom = "# ###,00 €";
            
            Console.WriteLine($"Formatted value: {cell.StringValue}");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


