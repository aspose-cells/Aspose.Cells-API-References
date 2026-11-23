---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Convertit la date et l'heure en valeur double"
type: docs
url: /fr/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Convertit la date‑heure en valeur double.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | La date et l'heure. |
| date1904 | Boolean | Système de date 1904. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // Créer une instance de classe Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la date et l'heure actuelles
            DateTime now = DateTime.Now;
            
            // Convertir DateTime en double à l'aide de CellsHelper
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // Définir la valeur dans la cellule A1
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // Formater la cellule pour l'afficher en tant que date
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


