---
title: "Cell.NumberCategoryType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Représente le type de catégorie du format numérique de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Représente le type de catégorie du format numérique de cette cellule.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Remarques

Lorsque le modèle de formatage d’une cellule est combiné avec des modèles de mise en forme conditionnelle, le type renvoyé correspond à la partie utilisée pour la valeur actuelle de cette cellule. Par exemple, si le modèle de formatage de cette cellule est "#,##0;(#,##0);"-";@", alors lorsque la valeur de la cellule est numérique et différente de 0, le type renvoyé est Number ; lorsque la valeur de la cellule est 0 ou n’est pas une valeur numérique, le type renvoyé est Text.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une valeur de date à la cellule A1
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // Définir le format de date
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // Ajouter une valeur numérique à la cellule A2
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // Ajouter une valeur texte à la cellule A3
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // Afficher NumberCategoryType pour chaque cellule
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // Modifier A2 en format monétaire et vérifier NumberCategoryType
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### Voir aussi

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


