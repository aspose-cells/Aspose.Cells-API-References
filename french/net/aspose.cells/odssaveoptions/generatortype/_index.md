---
title: "OdsSaveOptions.GeneratorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsSaveOptions. Obtient et définit le générateur du fichier ods"
type: docs
url: /fr/net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Obtient et définit le générateur du fichier ods.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyGeneratorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Créer et configurer les options d’enregistrement ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions
            {
                GeneratorType = OdsGeneratorType.LibreOffice,
                IsStrictSchema11 = true
            };

            // Enregistrer le classeur avec les options spécifiées
            workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Voir aussi

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


