---
title: "Validation.GetListValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Validation. Obtenir la valeur de la liste de la validation pour la cellule spécifiée"
type: docs
url: /fr/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Obtenez la valeur de la liste de validation pour la cellule spécifiée.

```csharp
public object GetListValue(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Valeur de retour

La valeur pour produire la liste de cette validation pour la cellule spécifiée. Si la liste fait référence à une plage, la valeur retournée sera un objet [`ReferredArea`](../../referredarea/); sinon la valeur retournée peut être null, object[], ou un objet simple.

### Remarques

Uniquement pour les validations dont le type est List et qui ont été appliquées à la cellule donnée, sinon null sera retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour la validation
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // Créer une validation pour la cellule B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // Tester GetListValue avec différents paramètres
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // Passer à des valeurs séparées par des virgules
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // Modifier en valeur unique
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


