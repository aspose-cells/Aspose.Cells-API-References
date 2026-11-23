---
title: "XlsbSaveOptions.CompressionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XlsbSaveOptions. Obtient et définit le type de compression pour le fichier ooxml"
type: docs
url: /fr/net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

Obtient et définit le type de compression pour le fichier ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Remarques

La valeur par défaut est OoxmlCompressionType.Level6.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyCompressionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Compression Test");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                CompressionType = OoxmlCompressionType.Level6
            };

            workbook.Save("XlsbWithCompression.xlsb", saveOptions);
        }
    }
}
```

### Voir aussi

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


