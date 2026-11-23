---
title: "ChartCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartCollection. Obtient l'élément Chart à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.charts/chartcollection/item/
---
## ChartCollection indexer (1 of 2)

Obtient l'élément [`Chart`](../../chart/) à l'index spécifié.

```csharp
public Chart this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            
            // Accéder au graphique en utilisant la propriété Item
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données et le titre du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Title.Text = "Sample Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Chart created successfully with Item property access.");
        }
    }
}
```

### Voir aussi

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ChartCollection indexer (2 of 2)

Obtient le graphique par son nom.

```csharp
public Chart this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom du graphique. |

### Valeur de retour

Le graphique.

### Remarques

Le nom de graphique par défaut est nul. Vous devez donc définir explicitement le nom du graphique.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Ajouter un graphique à la feuille de calcul
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);

                // Accédez au graphique en utilisant la propriété Item (indexeur)
                Chart chart = worksheet.Charts[chartIndex];

                // Afficher les informations sur le graphique
                Console.WriteLine("Chart type: " + chart.Type);
                Console.WriteLine("Chart name: " + chart.Name);

                // Enregistrez le classeur
                workbook.Save("ChartCollectionItemDemo.xlsx");

                Console.WriteLine("Chart created and accessed successfully using Item property.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


