---
title: "Protection.AllowInsertingHyperlink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si la inserción de hipervínculos está permitida en una hoja de cálculo protegida."
type: docs
url: /es/net/aspose.cells/protection/allowinsertinghyperlink/
---
## Protection.AllowInsertingHyperlink property

Representa si se permite la inserción de hipervínculos en una hoja de cálculo protegida

```csharp
public bool AllowInsertingHyperlink { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Protection protection = worksheet.Protection;
            protection.AllowInsertingHyperlink = true;
            protection.Password = "password123";

            // Agregar un hipervínculo para demostrar la funcionalidad
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


