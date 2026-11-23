---
title: "OoxmlSaveOptions.CompressionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OoxmlSaveOptions. Obtient et définit le type de compression pour le fichier ooxml"
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/compressiontype/
---
## OoxmlSaveOptions.CompressionType property

Obtient et définit le type de compression pour le fichier ooxml.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Remarques

La valeur par défaut est OoxmlCompressionType.Level2.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyCompressionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Compression Test");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;

            workbook.Save("CompressionDemo.xlsx", saveOptions);
            Console.WriteLine("Workbook saved with Level6 compression.");
        }
    }
}
```

### Voir aussi

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


