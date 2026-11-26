---
title: "Worksheet.PageSetup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Representa la descripción de la configuración de página en esta hoja"
type: docs
url: /es/net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Representa la descripción de la configuración de página en esta hoja.

```csharp
public PageSetup PageSetup { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer propiedades de configuración de página
            worksheet.PageSetup.PrintArea = "A1:L50";
            worksheet.PageSetup.PrintTitleRows = "1:2";
            worksheet.PageSetup.PrintTitleColumns = "A:B";
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
            
            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetupDemo.xlsx");
            
            Console.WriteLine("Worksheet page setup demo completed successfully.");
        }
    }
}
```

### Ver también

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


