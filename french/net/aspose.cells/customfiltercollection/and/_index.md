---
title: "CustomFilterCollection.And"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CustomFilterCollection. Indique si les deux critères ont une relation « et »"
type: docs
url: /fr/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

Indique si les deux critères ont une relation "et".

```csharp
public bool And { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
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
                // Créer une nouvelle CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Afficher la valeur par défaut de la propriété And
                Console.WriteLine($"Default And property value: {filters.And}");

                // Définir la propriété And sur true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // Définir la propriété And sur false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Enregistrez le classeur
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


