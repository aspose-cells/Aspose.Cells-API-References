---
title: "OdsSaveOptions.IsStrictSchema11"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsSaveOptions. Indica si el archivo ods debe guardarse como formato ODF versión 1.1. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/odssaveoptions/isstrictschema11/
---
## OdsSaveOptions.IsStrictSchema11 property

Indica si el archivo ods debe guardarse como formato ODF versión 1.1. El valor predeterminado es false.

```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad OdsSaveOptions.OdfStrictVersion. Este método será eliminado 12 meses después, a partir de febrero de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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

### Ver también

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


