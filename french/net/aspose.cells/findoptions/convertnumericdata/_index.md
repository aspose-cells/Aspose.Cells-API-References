---
title: "FindOptions.ConvertNumericData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Obtient ou définit une valeur qui indique si la conversion de la valeur de chaîne recherchée en données numériques doit être effectuée"
type: docs
url: /fr/net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Obtient ou définit une valeur qui indique si la conversion de la chaîne recherchée en données numériques est effectuée.

```csharp
public bool ConvertNumericData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple incluant des valeurs numériques sous forme de chaînes
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("456");
            worksheet.Cells["A3"].PutValue("01/28/2010");

            // Créer des options de recherche et définir ConvertNumericData sur true
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;

            // Trouver la valeur de date (stockée sous forme de chaîne mais convertie en numérique pendant la recherche)
            Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);

            // Afficher le résultat
            if (foundCell != null)
            {
                Console.WriteLine("Found value at: " + foundCell.Name);
                Console.WriteLine("Cell value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("Value not found");
            }
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


