---
title: "CopyOptions.CopyNames"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de CopyOptions. Indica si se copian los nombres"
type: docs
url: /es/net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

Indica si se copian los nombres.

```csharp
public bool CopyNames { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyNamesDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo de origen con rangos con nombre
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Cree un rango con nombre en el libro de trabajo de origen
            sourceSheet.Cells["A1"].PutValue("Test Value");
            int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
            sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            
            // Copie la hoja de cálculo con CopyNames=true
            destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });

            // Verifique que el rango con nombre se haya copiado
            Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
            if (copiedName != null)
            {
                Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
            }
            else
            {
                Console.WriteLine("Named range was not copied");
            }
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


