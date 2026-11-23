---
title: "JsonSaveOptions.ExportStylePool"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Indique s'il faut exporter les styles collectivement ou individuellement pour chaque cellule"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/exportstylepool/
---
## JsonSaveOptions.ExportStylePool property

Indique s’il faut exporter les styles collectivement ou individuellement pour chaque cellule.

```csharp
public bool ExportStylePool { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertyExportStylePoolDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d’exemple avec différents styles
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);

            // Appliquer différents styles aux cellules
            Aspose.Cells.Style style1 = workbook.CreateStyle();
            style1.Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(style1);

            Aspose.Cells.Style style2 = workbook.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Blue;
            worksheet.Cells["B1"].SetStyle(style2);

            try
            {
                // Créer JsonSaveOptions avec ExportStylePool = true (exportation collective)
                JsonSaveOptions options1 = new JsonSaveOptions();
                options1.ExportStylePool = true;
                Console.WriteLine("ExportStylePool (collective): " + options1.ExportStylePool);

                // Enregistrer avec une exportation de style collective
                workbook.Save("output_collective_styles.json", options1);

                // Créer JsonSaveOptions avec ExportStylePool = false (exportation individuelle)
                JsonSaveOptions options2 = new JsonSaveOptions();
                options2.ExportStylePool = false;
                Console.WriteLine("ExportStylePool (individual): " + options2.ExportStylePool);

                // Enregistrer avec une exportation de style individuelle
                workbook.Save("output_individual_styles.json", options2);

                Console.WriteLine("ExportStylePool demonstration completed successfully.");
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

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


