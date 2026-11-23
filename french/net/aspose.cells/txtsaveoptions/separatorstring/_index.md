---
title: "TxtSaveOptions.SeparatorString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtSaveOptions. Obtient et définit une valeur de chaîne comme séparateur"
type: docs
url: /fr/net/aspose.cells/txtsaveoptions/separatorstring/
---
## TxtSaveOptions.SeparatorString property

Obtient et définit une valeur chaîne comme séparateur.

```csharp
public string SeparatorString { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données de test
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue(2);

            // Enregistrer avec un séparateur d'espace
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = " ";
            workbook.Save("output_space.txt", saveOptions);

            // Enregistrer avec un séparateur pipe
            saveOptions.SeparatorString = "|";
            workbook.Save("output_pipe.txt", saveOptions);

            // Charger le fichier séparé par des espaces pour vérifier
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = " ";
            Workbook loadedWorkbook = new Workbook("output_space.txt", loadOptions);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;

            Console.WriteLine("Space-separated values:");
            Console.WriteLine($"{cells["A1"].StringValue} {cells["B1"].StringValue}");
            Console.WriteLine($"{cells["A2"].StringValue} {cells["B2"].StringValue}");
            Console.WriteLine($"{cells["A3"].IntValue} {cells["B3"].IntValue}");
        }
    }
}
```

### Voir aussi

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


