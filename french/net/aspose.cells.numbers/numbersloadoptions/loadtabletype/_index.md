---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NumbersLoadOptions. Obtient et définit le type de chargement de plusieurs tables dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Obtient et définit le type de chargement de plusieurs tables dans une feuille de calcul.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // Créer une instance de NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Démontrer l'utilisation de la propriété LoadTableType
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // Autres propriétés minimales requises
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // Charger un fichier Numbers avec les options de chargement spécifiées
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Enregistrer le classeur au format XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


