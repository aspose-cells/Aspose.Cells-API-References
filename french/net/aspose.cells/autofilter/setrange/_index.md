---
title: "AutoFilter.SetRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Définit la plage à laquelle le filtre automatique spécifié s'applique"
type: docs
url: /fr/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Définit la plage à laquelle le AutoFilter spécifié s'applique.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| startColumn | Int32 | Indice de colonne de départ. |
| endColumn | Int32 | Indice de la colonne de fin. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // Définir la plage du filtre automatique (firstRow, firstColumn, totalRows)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // Appliquer le filtre
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // Actualiser le filtre
            sheet.AutoFilter.Refresh();

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


