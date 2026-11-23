---
title: "SaveOptions.SortNames"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Indique s’il faut trier les noms définis avant d’enregistrer le fichier"
type: docs
url: /fr/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Indique si le tri des noms définis doit être effectué avant d'enregistrer le fichier.

```csharp
public bool SortNames { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // Créez un nouvel objet Workbook
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Créer une plage nommée
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // Créer des options d'enregistrement avec SortNames activé
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // Enregistrez le classeur
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


