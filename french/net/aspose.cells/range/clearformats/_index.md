---
title: "Range.ClearFormats"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Efface les formats de cette plage"
type: docs
url: /fr/net/aspose.cells/range/clearformats/
---
## Range.ClearFormats method

Efface les formats de cette plage.

```csharp
public void ClearFormats()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearFormatsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données avec mise en forme
            Cell cell = worksheet.Cells["A1"];
            cell.Value = "Formatted Cell";
            cell.GetStyle().Font.IsBold = true;
            cell.GetStyle().ForegroundColor = System.Drawing.Color.Yellow;
            cell.GetStyle().Pattern = BackgroundType.Solid;

            // Créez une plage
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B5");

            try
            {
                // Effacez les formats de la plage
                range.ClearFormats();

                Console.WriteLine("Formats cleared successfully from range A1:B5");
                Console.WriteLine($"Cell A1 value after clearing formats: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell A1 is bold after clearing formats: {worksheet.Cells["A1"].GetStyle().Font.IsBold}");

                // Enregistrez le classeur
                workbook.Save("ClearFormatsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearFormats: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


