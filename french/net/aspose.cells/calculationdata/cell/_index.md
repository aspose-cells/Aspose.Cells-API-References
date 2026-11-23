---
title: "CalculationData.Cell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationData. Obtient l'objet Cell où la fonction se trouve"
type: docs
url: /fr/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Obtient l'objet Cell où se trouve la fonction.

```csharp
public Cell Cell { get; }
```

### Remarques

Lors du calcul d'une formule sans l'affecter à une cellule, par exemple avec [`CalculateFormula`](../../worksheet/calculateformula/), la formule sera calculée comme si elle avait été placée dans la cellule A1, de sorte que [`CellRow`](../cellrow/) et [`CellColumn`](../cellcolumn/) sont tous deux à 0. Cependant, la cellule A1 de la feuille de calcul peut ne pas avoir été instanciée. Ainsi, dans ce type de situation, cette propriété sera nulle.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter des données pour rendre l’exemple significatif
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Créer des options de calcul avec un moteur personnalisé
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellDemoEngine();

                // Calculer les formules avec des options
                workbook.CalculateFormula(options);

                // Afficher le résultat
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Enregistrer le résultat
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Accéder à la propriété Cell en lecture seule
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


