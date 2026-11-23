---
title: "FormatCondition.SetFormula1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatCondition. Définit la valeur ou l'expression associée à cette condition de formatage"
type: docs
url: /fr/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

Définit la valeur ou l'expression associée à cette condition de format.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La valeur ou l'expression associée à cette condition de formatage. Si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon elle sera considérée comme une valeur simple (texte, nombre, bool). Pour une valeur texte qui commence par '=', l'utilisateur peut la saisir comme formule au format : \"=\\\"=...\\\"\". |
| isR1C1 | Boolean | Indique si la formule est une formule R1C1. |
| isLocal | Boolean | Si la formule est formatée selon la locale. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Ajouter une plage de formatage conditionnel
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtenir la première condition de formatage
            FormatCondition fc = fcc[0];

            try
            {
                // Appeler SetFormula1 avec des paramètres (String, Boolean, Boolean)
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // Afficher le résultat
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


