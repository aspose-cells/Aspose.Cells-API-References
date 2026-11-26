---
title: "PageSetup.IsHFDiffOddEven"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. True indica que el encabezado/pie de página de las páginas impares es diferente al de las páginas pares"
type: docs
url: /es/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

True significa que el encabezado/pie de página de las páginas impares es diferente al de las páginas impares.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Habilitar encabezados/pies de página diferentes para páginas impares y pares
            pageSetup.IsHFDiffOddEven = true;
            
            // Establecer pies de página diferentes para páginas impares y pares
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // Verificar la configuración cargando el archivo guardado
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


