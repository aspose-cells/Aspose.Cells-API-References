---
title: "WorkbookSettings.CultureInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit les informations de culture du système"
type: docs
url: /fr/net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Obtient ou définit les informations de culture du système.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Remarques

Renvoie null si les informations de culture ne sont pas définies et que [`Region`](../region/) n'est pas définie.

### Exemples

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
            // Créer un classeur
            Workbook wb = new Workbook();
            
            // Définir la région sur la France pour démontrer les changements de CultureInfo
            wb.Settings.Region = CountryCode.France;
            
            // Obtenir le séparateur de groupe de la culture française
            string groupSep = wb.Settings.CultureInfo.NumberFormat.NumberGroupSeparator;
            Console.WriteLine($"French group separator: '{groupSep}'");
            
            // Créer un style avec un format personnalisé et afficher le format adapté à la culture
            Style style = wb.CreateStyle();
            style.Custom = "#,##0.00_ ;-#,##0.00";
            Console.WriteLine($"Culture-adjusted custom format: {style.CultureCustom}");
            
            // Démontrer le formatage des nombres avec la culture française
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

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


