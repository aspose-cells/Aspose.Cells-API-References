---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SpreadsheetML2003SaveOptions. El valor predeterminado es false, lo que significa que el índice de columna se ignorará si la celda es contigua a la celda anterior"
type: docs
url: /es/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

El valor predeterminado es false, lo que significa que el índice de columna se ignorará si la celda es contigua a la celda anterior.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
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
            
            // Crear opciones de guardado con ExportColumnIndexOfCell habilitado
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // Guardar el libro de trabajo con información del índice de columna
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### Ver también

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


