---
title: "Cells.TextToColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Divise le contenu de la colonne spécifiée en plusieurs colonnes"
type: docs
url: /fr/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Divise le contenu de la colonne spécifiée en plusieurs colonnes..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |
| totalRows | Int32 | Le nombre de lignes. |
| options | TxtLoadOptions | Les options de division. |

### Valeur de retour

Nombre total de colonnes des valeurs divisées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir des données d'exemple avec des valeurs séparées par des virgules
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // Créer des options de chargement de texte avec la virgule comme séparateur
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // Diviser le texte en colonnes à partir de la cellule A1, sur 3 colonnes de largeur
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // Vérifier les résultats
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


