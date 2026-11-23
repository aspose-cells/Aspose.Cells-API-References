---
title: "ImportTableOptions.ConvertNumericData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Obtient ou définit une valeur indiquant si la valeur chaîne doit être convertie en valeur numérique ou date"
type: docs
url: /fr/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Obtient ou définit une valeur qui indique si la valeur chaîne doit être convertie en valeur numérique ou date.

```csharp
public bool ConvertNumericData { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer un tableau de données d'exemple avec des valeurs numériques et des chaînes
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // Obtenir les cellules de la première feuille de calcul
            Cells cells = workbook.Worksheets[0].Cells;

            // Créer des options d'importation avec ConvertNumericData défini sur true
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // Importer des données avec conversion numérique
            cells.ImportData(dt, 0, 0, options);

            // Afficher les résultats
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


