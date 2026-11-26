---
title: "WorkbookSettings.NumberDecimalSeparator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece el separador decimal para formatear/analizar valores numéricos. El valor predeterminado es el separador decimal de la región actual"
type: docs
url: /es/net/aspose.cells/workbooksettings/numberdecimalseparator/
---
## WorkbookSettings.NumberDecimalSeparator property

Obtiene o establece el separador decimal para formatear/analizar valores numéricos. El predeterminado es el separador decimal de la región actual.

```csharp
public char NumberDecimalSeparator { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyNumberDecimalSeparatorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.NumberDecimalSeparator = ',';
            wb.Settings.NumberGroupSeparator = '.';
            
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00";
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(12345.6798);
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


