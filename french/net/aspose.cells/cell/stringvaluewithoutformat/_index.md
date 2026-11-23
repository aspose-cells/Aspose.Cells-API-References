---
title: "Cell.StringValueWithoutFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la valeur de la cellule sous forme de chaîne sans aucun format"
type: docs
url: /fr/net/aspose.cells/cell/stringvaluewithoutformat/
---
## Cell.StringValueWithoutFormat property

Obtient la valeur de la cellule sous forme de chaîne sans aucun format.

```csharp
[Obsolete("Use GetStringValue(CellValueFormatStrategy) with CellValueFormatStrategy.None instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValueWithoutFormat { get; }
```

### Remarques

NOTE: Cette méthode est désormais obsolète. À la place, l'utilisateur doit obtenir l'objet valeur et le formater selon le type de valeur et les exigences spécifiques. Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2020. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyStringValueWithoutFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter différents types de données pour démontrer StringValueWithoutFormat
            worksheet.Cells["A1"].PutValue("Plain Text");
            worksheet.Cells["A2"].PutValue(12345);
            worksheet.Cells["A3"].PutValue(3.14159);
            worksheet.Cells["A4"].PutValue(DateTime.Now);

            // Appliquer le formatage numérique à certaines cellules
            Style style = worksheet.Cells["A2"].GetStyle();
            style.Number = 3; // Currency format
            worksheet.Cells["A2"].SetStyle(style);

            style = worksheet.Cells["A3"].GetStyle();
            style.Number = 9; // Percentage format
            worksheet.Cells["A3"].SetStyle(style);

            try
            {
                // Afficher StringValueWithoutFormat pour chaque cellule
                Console.WriteLine("A1 StringValueWithoutFormat: " + worksheet.Cells["A1"].StringValueWithoutFormat);
                Console.WriteLine("A2 StringValueWithoutFormat: " + worksheet.Cells["A2"].StringValueWithoutFormat);
                Console.WriteLine("A3 StringValueWithoutFormat: " + worksheet.Cells["A3"].StringValueWithoutFormat);
                Console.WriteLine("A4 StringValueWithoutFormat: " + worksheet.Cells["A4"].StringValueWithoutFormat);

                // Comparer avec la StringValue formatée
                Console.WriteLine("\nComparison with formatted values:");
                Console.WriteLine("A2 StringValue (formatted): " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3 StringValue (formatted): " + worksheet.Cells["A3"].StringValue);

                // Enregistrez le classeur
                workbook.Save("StringValueWithoutFormatDemo.xlsx");
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


