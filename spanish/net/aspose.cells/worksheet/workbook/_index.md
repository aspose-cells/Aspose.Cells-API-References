---
title: "Worksheet.Workbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene el objeto de libro de trabajo que contiene esta hoja"
type: docs
url: /es/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Obtiene el objeto del libro de trabajo que contiene esta hoja.

```csharp
public Workbook Workbook { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo fuente y obtener una hoja de cálculo
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo fuente
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            
            // Copiar el tema del libro de trabajo fuente usando la propiedad Worksheet.Workbook
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // Acceder a la hoja de cálculo de destino y copiar datos
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // Copiar datos con formato
            destRange.Copy(sourceRange);
            
            // Guardar el libro de trabajo de destino
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


