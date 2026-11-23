---
title: "TxtSaveOptions.TrimTailingBlankCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtSaveOptions. Indique si les cellules vides en fin de ligne doivent être supprimées. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

Indique si les cellules vides en fin de ligne doivent être supprimées. La valeur par défaut est false.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### Remarques

Lors de l’enregistrement en mode LightCells et que [`ExportArea`](../exportarea/) n’a pas été spécifié, cette option n’a aucun effet et une ligne sera étendue jusqu’à la dernière cellule fournie par l’implémentation [`LightCellsDataProvider`](../lightcellsdataprovider/)

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Ajoutez des données d'exemple
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[0, 2].PutValue("C");
            cells[1, 0].PutValue(1);
            cells[1, 2].PutValue(2);
            cells[2, 0].PutValue(3);

            // Enregistrez sans supprimer les cellules vides en fin de ligne (par défaut)
            TxtSaveOptions options1 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = false
            };
            string result1 = SaveAsCsv(workbook, options1);
            Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);

            // Enregistrez en supprimant les cellules vides en fin de ligne
            TxtSaveOptions options2 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = true
            };
            string result2 = SaveAsCsv(workbook, options2);
            Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
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


