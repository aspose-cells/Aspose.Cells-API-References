---
title: "Workbook.SaveToStream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Guarda el archivo Excel en un objeto MemoryStream como un archivo Excel972003 xls y lo devuelve"
type: docs
url: /es/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Guarda el archivo Excel en un objeto MemoryStream como un archivo xls de Excel97-2003 y lo devuelve.

```csharp
public MemoryStream SaveToStream()
```

### Valor de retorno

Objeto MemoryStream que contiene un archivo Excel xls.

### Observaciones

Este método proporciona la misma función que el método Save y solo guarda el libro de trabajo como archivo Excel97-2003 xls. Está pensado principalmente para ser llamado desde clientes COM.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook start = new Workbook();
            
            // Acceder a la primera hoja y agregar algunos datos de muestra
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Guardar el libro de trabajo en un flujo de memoria
            MemoryStream stream = start.SaveToStream();

            // Crear un nuevo libro de trabajo a partir del flujo
            Workbook workbook = new Workbook(stream);

            // Modificar el nuevo libro de trabajo
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // Guardar el libro de trabajo modificado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


