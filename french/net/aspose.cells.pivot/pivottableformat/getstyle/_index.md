---
title: "PivotTableFormat.GetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTableFormat. Obtient le style formaté"
type: docs
url: /fr/net/aspose.cells.pivot/pivottableformat/getstyle/
---
## PivotTableFormat.GetStyle method

Obtient le style formaté.

```csharp
public Style GetStyle()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableFormatMethodGetStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtenez le format du tableau pivot
            PivotTableFormatCollection formats = pivotTable.PivotFormats;
            PivotTableFormat format = formats[0];

            try
            {
                // Appelez la méthode GetStyle
                Style style = format.GetStyle();

                // Propriétés du style d'affichage
                Console.WriteLine("Style properties:");
                Console.WriteLine($"Font Name: {style.Font.Name}");
                Console.WriteLine($"Font Size: {style.Font.Size}");
                Console.WriteLine($"Background Color: {style.BackgroundColor}");

                // Modifier le style
                style.Font.Name = "Arial";
                style.Font.Size = 12;
                style.BackgroundColor = System.Drawing.Color.LightBlue;

                // Appliquez le style modifié au format
                format.SetStyle(style);

                Console.WriteLine("GetStyle method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStyle method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("PivotTableFormatMethodGetStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


