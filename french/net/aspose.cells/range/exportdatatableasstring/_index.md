---
title: "Range.ExportDataTableAsString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Exporte les données de cette plage vers un objet DataTable"
type: docs
url: /fr/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

Exporte les données de cette plage vers un objet DataTable.

```csharp
public DataTable ExportDataTableAsString()
```

### Valeur de retour

Objet DataTable exporté.

### Remarques

Toutes les données de la collection [`Cells`](../../cells/) sont converties en chaînes.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableAsStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // Obtenir la plage contenant les données
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // Appeler la méthode ExportDataTableAsString
                DataTable dataTable = range.ExportDataTableAsString();

                // Afficher les données exportées
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // Enregistrez le classeur
                workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


