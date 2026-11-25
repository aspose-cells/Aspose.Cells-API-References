---
title: "WorkbookSettings.CultureInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta le informazioni sulla cultura di sistema"
type: docs
url: /it/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Ottiene o imposta le informazioni sulla cultura di sistema.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Osservazioni

Restituisce null se le informazioni sulla cultura non sono impostate e [`Region`](../region/) non è impostata.

### Esempi

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
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            
            // Imposta la regione su Francia per dimostrare le modifiche di CultureInfo
            wb.Settings.Region = CountryCode.France;
            
            // Ottieni il separatore di gruppo dalla cultura francese
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // Crea uno stile con formato personalizzato e mostra il formato adattato alla cultura
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // Dimostra la formattazione dei numeri con la cultura francese
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

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


