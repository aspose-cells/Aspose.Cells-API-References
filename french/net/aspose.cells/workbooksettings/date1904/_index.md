---
title: "WorkbookSettings.Date1904"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit une valeur indiquant si le classeur utilise le système de dates 1904"
type: docs
url: /fr/net/aspose.cells/workbooksettings/date1904/
---
## WorkbookSettings.Date1904 property

Obtient ou définit une valeur indiquant si le workbook utilise le système de dates 1904.

```csharp
public bool Date1904 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDate1904Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Date1904 = true;

            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Démontrer le temps négatif avec Date1904
            Style style = cell.GetStyle();
            style.Custom = "h:mm";
            cell.SetStyle(style);
            cell.PutValue(-0.0736111111111112);
            Console.WriteLine("Negative time value: " + cell.DisplayStringValue);

            // Démontrer la date négative avec Date1904
            style = cell.GetStyle();
            style.Custom = "mm/dd/yyyy h:mm:ss";
            cell.SetStyle(style);
            cell.PutValue(-42389.47075706);
            Console.WriteLine("Negative date value: " + cell.DisplayStringValue);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


