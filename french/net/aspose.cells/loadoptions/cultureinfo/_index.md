---
title: "LoadOptions.CultureInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé"
type: docs
url: /fr/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Remarques

Cette propriété a le même effet que [`Region`](../region/) pour définir les paramètres régionaux.

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Créer un fichier Excel d'exemple
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // Charger avec une culture spécifique
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


