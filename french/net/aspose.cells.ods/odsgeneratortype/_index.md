---
title: "Énum OdsGeneratorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "enum Aspose.Cells.Ods.OdsGeneratorType. Représente le type de générateur ODS"
type: docs
url: /fr/net/aspose.cells.ods/odsgeneratortype/
---
## OdsGeneratorType enumeration

Représente le type de générateur ODS.

```csharp
public enum OdsGeneratorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LibreOffice | `0` | Libre Office |
| OpenOffice | `1` | Open Office |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsClassOdsGeneratorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
            
            workbook.Save("OdsGeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


