---
title: "Cells.IsBlankColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Vérifie si la colonne donnée est vide et ne contient aucune donnée"
type: docs
url: /fr/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Vérifie si la colonne donnée est vide (ne contient aucune donnée).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | l'index de la colonne |

### Valeur de retour

vrai si la colonne donnée ne contient aucune donnée

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Vérifier si la colonne 2 est vide (devrait être vrai pour une nouvelle feuille de calcul)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // Ajouter des données à la colonne 2
            worksheet.Cells["B1"].PutValue("Test Data");

            // Vérifier à nouveau (devrait maintenant être faux)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // Créer une autre feuille de calcul avec des colonnes entièrement vides
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // Vérifier une colonne dans la feuille de calcul vide (devrait être vrai)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


