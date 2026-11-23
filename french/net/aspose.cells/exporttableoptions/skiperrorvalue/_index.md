---
title: "ExportTableOptions.SkipErrorValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ExportTableOptions property. Indique si l’on doit ignorer les valeurs invalides pour la colonne. Par exemple, si le type de colonne est décimal, que la valeur est supérieure à decimal.MaxValue et que cette propriété est true, nous ne lancerons plus d’exception. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

Indique s'il faut ignorer les valeurs invalides pour la colonne. Par exemple, si le type de la colonne est décimal, que la valeur dépasse decimal.MaxValue et que cette propriété est true, nous ne lancerons plus d'exception. La valeur par défaut est false.

```csharp
public bool SkipErrorValue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertySkipErrorValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;

            Worksheet ws = wb.Worksheets[0];

            // Premier cas de test - valeurs numériques
            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
            Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56

            // Deuxième cas de test - valeurs mixtes
            ws.Cells["A2"].Value = "dummy";
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"

            // Troisième cas de test - exportation en tant que chaîne
            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


