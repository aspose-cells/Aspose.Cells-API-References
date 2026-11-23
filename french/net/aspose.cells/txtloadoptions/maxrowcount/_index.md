---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Le nombre maximal de lignes à importer pour une feuille"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

Le nombre maximal de lignes à importer pour une feuille.

```csharp
public int MaxRowCount { get; set; }
```

### Remarques

Les lignes dépassant cette limite seront ignorées ou prolongées vers la feuille suivante selon [`ExtendToNextSheet`](../extendtonextsheet/). Ce nombre inclut les lignes d'en-tête ([`HeaderRowsCount`](../headerrowscount/)). La valeur maximale autorisée est la limite de lignes du format de fichier correspondant, par exemple pour le fichier xlsx elle est de 1048576. Si cette propriété n'a pas été spécifiée ou si la valeur spécifiée n'est pas positive, la limite maximale sera également utilisée.

### Exemples

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // Créez un contenu CSV d'exemple
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // Créer TxtLoadOptions avec MaxRowCount défini à 4
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // Charger le CSV dans le classeur
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // Vérifier que seules 4 lignes ont été chargées (1 en-tête + 3 lignes de données)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // Cela serait nul puisque nous n'avons chargé que 4 lignes (index 0-3)
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
                }
            }
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


