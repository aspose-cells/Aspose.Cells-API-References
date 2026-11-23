---
title: "Cells.GetLastDataRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l'index de la dernière ligne de cellule contenant des données dans la colonne spécifiée"
type: docs
url: /fr/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Obtient l'index de la dernière ligne de la cellule qui contient des données dans la colonne spécifiée.

```csharp
public int GetLastDataRow(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |

### Valeur de retour

index de la dernière ligne.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // Obtenir la dernière ligne de données dans la colonne A (index 0)
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // Afficher le résultat
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // Insérer une nouvelle ligne après la dernière ligne de données
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // Ajouter des données à la nouvelle ligne
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


