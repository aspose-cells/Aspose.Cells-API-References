---
title: "Worksheet.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet propiedad. Representa el tipo de Worksheet"
type: docs
url: /es/net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Representa el tipo de hoja de cálculo.

```csharp
public SheetType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer algunas propiedades básicas
            worksheet.Name = "DemoSheet";
            worksheet.IsVisible = true;
            
            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Worksheet Type: " + worksheet.Type);
            
            // Agregar una hoja de gráfico para demostrar diferentes tipos de worksheet
            workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[1];
            
            // Comparar tipos de worksheet
            Console.WriteLine("Regular Sheet Type: " + worksheet.Type);
            Console.WriteLine("Chart Sheet Type: " + chartSheet.Type);
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


