---
title: "PageSetup.Order"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PageSetup property. Representa el orden que Microsoft Excel usa para numerar páginas al imprimir una hoja de cálculo grande"
type: docs
url: /es/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Representa el orden que Microsoft Excel usa para numerar las páginas al imprimir una hoja de cálculo grande.

```csharp
public PrintOrderType Order { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer el orden de impresión a DownThenOver
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // Guarde el libro de trabajo en diferentes formatos
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // Cambie el orden de impresión a OverThenDown
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // Guarde nuevamente con diferentes formatos
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### Ver también

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


