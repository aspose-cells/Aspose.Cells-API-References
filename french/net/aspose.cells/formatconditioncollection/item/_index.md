---
title: "FormatConditionCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatConditionCollection. Obtient la condition de formatage par indice"
type: docs
url: /fr/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Obtient la condition de formatage par index.

```csharp
public FormatCondition this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | l'indice de la condition de formatage à retourner. |

### Valeur de retour

la condition de formatage

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une collection de conditions de formatage
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Ajouter une condition de formatage
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // Accéder à la première condition de formatage en utilisant la propriété Item
            FormatCondition condition = fcc[0];
            
            // Afficher les formules
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // Modifier les formules en utilisant la propriété Item
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // Afficher les formules modifiées
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


