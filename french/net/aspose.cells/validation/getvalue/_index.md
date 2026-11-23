---
title: "Validation.GetValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Validation. Obtenir la valeur de la validation sur la cellule spécifique"
type: docs
url: /fr/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Obtenez la valeur de la validation sur la cellule spécifique.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |
| isValue1 | Boolean | Indique si la première valeur est obtenue. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et une validation
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // Créer une validation pour la cellule B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // Obtenir la valeur en utilisant la méthode GetValue avec les paramètres ligne, colonne et convertir le numérique en date
            object value = validation.GetValue(0, 1, false);
            
            // Afficher le résultat
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


