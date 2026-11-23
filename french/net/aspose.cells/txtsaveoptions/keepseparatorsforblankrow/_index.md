---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtSaveOptions. Indique si les séparateurs doivent être générés pour une ligne vide. La valeur par défaut est false, ainsi le contenu d'une ligne vide sera vide."
type: docs
url: /fr/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Indique si des séparateurs doivent être générés pour une ligne vide. La valeur par défaut est false, ainsi le contenu d'une ligne vide sera vide.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Ajoutez des données avec des lignes vides
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // Créer des options d'enregistrement avec KeepSeparatorsForBlankRow défini sur true
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // Enregistrez le classeur au format CSV avec les options
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### Voir aussi

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


