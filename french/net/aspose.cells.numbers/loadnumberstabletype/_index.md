---
title: "Enum LoadNumbersTableType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Numbers.LoadNumbersTableType enum. Indique le type de chargement des tables lorsque certaines tables sont dans une feuille."
type: docs
url: /fr/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

Indique le type de chargement des tables lorsque certaines tables sont dans une feuille.

```csharp
public enum LoadNumbersTableType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;

    public class LoadNumbersTableTypeDemo
    {
        public static void LoadNumbersTableTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une nouvelle feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // Définir la propriété LoadNumbersTableType
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // Charger un fichier Numbers avec les options de chargement spécifiées
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


