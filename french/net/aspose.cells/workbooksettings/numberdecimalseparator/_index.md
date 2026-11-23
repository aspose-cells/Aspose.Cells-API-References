---
title: "WorkbookSettings.NumberDecimalSeparator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle"
type: docs
url: /fr/net/aspose.cells/workbooksettings/numberdecimalseparator/
---
## WorkbookSettings.NumberDecimalSeparator property

Obtient ou définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle.

```csharp
public char NumberDecimalSeparator { get; set; }
```

### Exemples

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

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


