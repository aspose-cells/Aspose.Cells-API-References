---
title: "CalculationData.ParamCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationData. Obtient le nombre de paramètres"
type: docs
url: /fr/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Obtient le nombre de paramètres

```csharp
public int ParamCount { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur et obtenez la première feuille de calcul
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Remplir certaines cellules qui seront utilisées comme paramètres
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Définir une formule qui appelle une fonction personnalisée avec trois arguments
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Configurer les options de calcul pour utiliser un moteur personnalisé
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Effectuer le calcul
                workbook.CalculateFormula(options);

                // Le moteur personnalisé renvoie le ParamCount comme valeur calculée
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // Enregistrer le classeur de façon optionnelle
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Moteur de calcul personnalisé qui montre la lecture de la propriété ParamCount
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Identifier la fonction personnalisée par son nom
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Lire la propriété ParamCount en lecture seule
                    int count = data.ParamCount;

                    // Utiliser le compte comme résultat de la fonction
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### Voir aussi

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


