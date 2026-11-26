---
title: "Workbook.Worksheets"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene la colección WorksheetCollection en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Obtiene la colección [`WorksheetCollection`](../../worksheetcollection/) en la hoja de cálculo.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Valor de retorno

[`WorksheetCollection`](../../worksheetcollection/) collection

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Agregar una nueva hoja de trabajo
            workbook.Worksheets.Add("SecondSheet");
            
            // Acceder a la segunda hoja de cálculo y agregar datos
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // Guarda el libro de trabajo
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // Mostrar el recuento de hojas de cálculo
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


