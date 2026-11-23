---
title: "ImportTableOptions.Styles"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Obtient et définit les styles pour chaque colonne du tableau"
type: docs
url: /fr/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

Obtient et définit les styles pour chaque colonne du tableau.

```csharp
public Style[] Styles { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyStylesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une table de données d'exemple
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // Créer ImportTableOptions et définir la propriété Styles
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // Créer des styles pour chaque colonne
                Style[] columnStyles = new Style[2];

                // Style pour la colonne Produit (gras, police bleue)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Style pour la colonne Prix (format monétaire, police verte)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // Définir la propriété Styles
                options.Styles = columnStyles;

                // Importer des données avec des styles
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // Afficher les styles appliqués
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // Enregistrez le classeur
                workbook.Save("StylesDemo.xlsx");
                Console.WriteLine("Workbook saved with styled data.");
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

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


