---
title: "Enum PivotTableSourceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Pivot.PivotTableSourceType. Représente le type de source de données du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

Représente le type de source de données du tableau croisé dynamique.

```csharp
public enum PivotTableSourceType : byte
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Sheet | `1` | Spécifie que les données source sont une plage. |
| External | `2` | Spécifie que des données source externes sont utilisées. |
| Consolidation | `4` | Spécifie que plusieurs plages de consolidation sont utilisées comme données source. |
| Scenario | `8` | Les données source sont remplies à partir d'une structure interne temporaire. |
| Unknown | `9` | Source de données inconnue. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données d'exemple à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Créer une collection de tableaux croisés dynamiques
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Ajouter un tableau croisé dynamique en utilisant la feuille comme type de source
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Afficher le type de source
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Démontrer différents types de source
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Enregistrez le classeur
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


