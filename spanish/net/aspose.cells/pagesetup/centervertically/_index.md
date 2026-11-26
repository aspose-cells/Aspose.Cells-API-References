---
title: "PageSetup.CenterVertically"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Indica si la hoja se imprime centrada verticalmente"
type: docs
url: /es/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Representa si la hoja se imprime centrada verticalmente.

```csharp
public bool CenterVertically { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a PageSetup y establecer CenterVertically
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // Agregar algunos datos de ejemplo para visualizar el efecto
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


