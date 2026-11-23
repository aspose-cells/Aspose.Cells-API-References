---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur NumbersLoadOptions. Constructeur"
type: docs
url: /fr/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

Constructeur.

```csharp
public NumbersLoadOptions()
```

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer NumbersLoadOptions en utilisant le constructeur
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Définir quelques propriétés communes
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // Chargez le classeur avec les options
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Enregistrer au format XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


