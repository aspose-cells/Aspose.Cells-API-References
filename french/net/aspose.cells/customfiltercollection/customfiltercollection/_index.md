---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur CustomFilterCollection. Construit une nouvelle instance"
type: docs
url: /fr/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Construit une nouvelle instance.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez définir FilterColumn.FilterType sur FilterType.CustomFilters puis récupérer FilterColumn.CustomFilters. Cette propriété sera supprimée 12 mois plus tard, à compter de juin 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Créer une nouvelle CustomFilterCollection en utilisant le constructeur
                CustomFilterCollection filters = new CustomFilterCollection();

                // Afficher la valeur par défaut de la propriété And
                Console.WriteLine($"Default And property value: {filters.And}");

                // Le constructeur crée une collection vide
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Enregistrez le classeur
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


