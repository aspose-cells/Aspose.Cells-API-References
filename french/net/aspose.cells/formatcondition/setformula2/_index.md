---
title: "FormatCondition.SetFormula2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatCondition. Définit la valeur ou l'expression associée à cette condition de formatage"
type: docs
url: /fr/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

Définit la valeur ou l'expression associée à cette condition de format.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
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

            // Ajouter une condition de formatage
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtenir la première condition de formatage
            FormatCondition fc = fcs[0];

            try
            {
                // Appeler SetFormula2 avec les paramètres (String, Boolean, Boolean)
                fc.SetFormula2("25", false, false);

                // Afficher le résultat
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // Appliquer un style pour rendre l'effet visible
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


