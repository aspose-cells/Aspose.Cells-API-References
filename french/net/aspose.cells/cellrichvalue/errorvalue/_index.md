---
title: "CellRichValue.ErrorValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellRichValue. Obtient le type de valeur d'erreur de la cellule"
type: docs
url: /fr/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Obtient le type de valeur d'erreur de la cellule.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une erreur de débordement dans la cellule A1
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // Calculer les formules pour générer l'erreur de débordement
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Erreur de débordement attendue
            }
            
            // Obtenir la valeur riche de la cellule A1
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Vérifier et afficher le type d'erreur
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


