---
title: "LoadOptions.FontConfigs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient et définit les configurations de police individuelles. Ne fonctionne que pour le Workbook qui utilise ces LoadOptions pour le chargement"
type: docs
url: /fr/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

Obtient et définit les configurations de police individuelles. Ne fonctionne que pour le [`Workbook`](../../workbook/) qui utilise ce [`LoadOptions`](../) pour charger.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyFontConfigsDemo
    {
        public static void Run()
        {
            // Créez des options de chargement avec FontConfigs
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // Définissez des règles de substitution de police en utilisant l'API correcte
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // Charger un fichier CSV avec les options spécifiées
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


