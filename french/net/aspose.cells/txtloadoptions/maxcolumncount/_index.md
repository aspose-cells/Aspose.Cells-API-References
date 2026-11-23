---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Le nombre maximal de colonnes à importer pour une feuille"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

Le nombre maximal de colonnes à importer pour une feuille.

```csharp
public int MaxColumnCount { get; set; }
```

### Remarques

Les colonnes dépassant cette limite seront ignorées ou prolongées vers la feuille suivante selon [`ExtendToNextSheet`](../extendtonextsheet/). Ce nombre inclut les colonnes d'en-tête ([`HeaderColumnsCount`](../headercolumnscount/)). La valeur maximale est la limite de colonnes du format de fichier correspondant, par exemple pour le fichier xlsx elle est de 16384. Si cette propriété n'a pas été spécifiée ou si la valeur spécifiée n'est pas positive, la limite maximale sera également utilisée.

### Exemples

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxColumnCountDemo
    {
        public static void Run()
        {
            // Créez un contenu CSV d'exemple
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // Créer TxtLoadOptions avec MaxColumnCount défini à 5
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // Charger le CSV avec des colonnes limitées
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Afficher les données chargées (seules les 5 premières colonnes doivent être présentes)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Vérifier que seules 5 colonnes ont été chargées
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


