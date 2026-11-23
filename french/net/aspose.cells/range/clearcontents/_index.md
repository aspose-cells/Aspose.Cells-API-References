---
title: "Range.ClearContents"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Efface le contenu de cette plage"
type: docs
url: /fr/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

Efface le contenu de cette plage.

```csharp
public void ClearContents()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour démontrer le nettoyage
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // Créez une plage couvrant les cellules A1:B2
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Affichez le contenu de la plage avant le nettoyage
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Appelez ClearContents pour supprimer toutes les valeurs de la plage
                range.ClearContents();

                // Affichez le contenu de la plage après le nettoyage
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Enregistrez le classeur
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


