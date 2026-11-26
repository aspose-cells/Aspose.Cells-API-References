---
title: "PageSetup.IsAutoFirstPageNumber"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Indica si el número de página inicial se asigna automáticamente"
type: docs
url: /es/net/aspose.cells/pagesetup/isautofirstpagenumber/
---
## PageSetup.IsAutoFirstPageNumber property

Indica si el número de la primera página se asigna automáticamente.

```csharp
public bool IsAutoFirstPageNumber { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutoFirstPageNumberDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer propiedades de configuración de página
            worksheet.PageSetup.IsAutoFirstPageNumber = true;
            Console.WriteLine("Auto First Page Number (Worksheet 1): " + worksheet.PageSetup.IsAutoFirstPageNumber);

            // Agregar una segunda hoja de cálculo
            worksheet = workbook.Worksheets.Add("Sheet2");
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            Console.WriteLine("Auto First Page Number (Worksheet 2): " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("First Page Number (Worksheet 2): " + worksheet.PageSetup.FirstPageNumber);

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_IsAutoFirstPageNumber_Example.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


