---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractTextLoadOptions. Indique s’il ne faut pas analyser une chaîne si sa longueur est de 15"
type: docs
url: /fr/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15.

```csharp
public bool KeepPrecision { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // Créez des options de chargement HTML et définissez KeepPrecision sur true
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // Chargez le classeur avec les options
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontrez que la précision est conservée (par ex., valeurs numériques avec de nombreuses décimales)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


