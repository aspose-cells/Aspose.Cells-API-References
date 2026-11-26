---
title: "TxtSaveOptions.ExportArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. El rango de celdas a exportar"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/exportarea/
---
## TxtSaveOptions.ExportArea property

El rango de celdas a exportar.

```csharp
public CellArea ExportArea { get; set; }
```

### Observaciones

Si se ha especificado el área exportada, [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) no tendrá efecto.

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellene las celdas con datos
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(699.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(399.99);

            // Configure las opciones de guardado de texto con ExportArea
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = '\t',
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Guarde solo el área especificada (primeras 3 filas, primeras 2 columnas)
            workbook.Save("ExportedData.txt", saveOptions);

            Console.WriteLine("Data exported successfully with ExportArea restriction.");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


