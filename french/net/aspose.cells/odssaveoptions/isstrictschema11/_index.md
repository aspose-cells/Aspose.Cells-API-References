---
title: "OdsSaveOptions.IsStrictSchema11"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsSaveOptions. Indique si le fichier ods doit être enregistré au format ODF version 1.1. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/odssaveoptions/isstrictschema11/
---
## OdsSaveOptions.IsStrictSchema11 property

Indique si le fichier ods doit être enregistré au format ODF version 1.1. La valeur par défaut est false.

```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété OdsSaveOptions.OdfStrictVersion. Cette méthode sera supprimée 12 mois plus tard, depuis février 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyIsStrictSchema11Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample ODS with strict schema");

            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.IsStrictSchema11 = true;
            
            workbook.Save("StrictSchema11Example.ods", saveOptions);
        }
    }
}
```

### Voir aussi

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


