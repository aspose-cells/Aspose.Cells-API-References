---
title: "Cell.HasCustomStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si cette cellule possède des paramètres de style personnalisés différents de ceux par défaut hérités de la ligne, de la colonne ou du classeur correspondant"
type: docs
url: /fr/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

Indique si cette cellule possède des paramètres de style personnalisés (différents de ceux par défaut hérités de la ligne, de la colonne ou du classeur correspondants).

```csharp
public bool HasCustomStyle { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // Affichez la valeur initiale de HasCustomState (hérite du style par défaut)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // Créez un style personnalisé et appliquez-le à la cellule
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // Vérifiez que HasCustomStyle est vrai après la modification du style
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // Enregistrez le classeur avec le style personnalisé appliqué
            workbook.Save("CellCustomStyleDemo.xlsx");

            // Réinitialisez le style de la cellule au style par défaut du classeur
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // Vérifiez que HasCustomStyle est faux après être revenu au style par défaut
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


