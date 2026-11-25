---
title: "OdsSaveOptions.IsStrictSchema11"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsSaveOptions. Indica se il file ods deve essere salvato come formato ODF versione 1.1. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/odssaveoptions/isstrictschema11/
---
## OdsSaveOptions.IsStrictSchema11 property

Indica se il file ods deve essere salvato come formato ODF versione 1.1. Il valore predefinito è false.

```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà OdsSaveOptions.OdfStrictVersion. Questo metodo sarà rimosso 12 mesi dopo a partire da febbraio 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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

### Vedi anche

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


