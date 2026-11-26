---
title: "ImportTableOptions.CheckMergedCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Indica si se verifica la existencia de celdas combinadas"
type: docs
url: /es/net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Indica si se deben comprobar celdas combinadas.

```csharp
public bool CheckMergedCells { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Customer1
    {
        public int CustomerId { get; set; }
        public string Name { get; set; }
    }

    public class ImportTableOptionsPropertyCheckMergedCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear celdas combinadas para demostración
            worksheet.Cells.Merge(3, 3, 2, 1); // Merge D4:D5
            worksheet.Cells[3, 3].PutValue("MergedValue");

            // Crear datos de ejemplo
            List<Customer1> customers = new List<Customer1>
            {
                new Customer1 { CustomerId = 1, Name = "Customer1" },
                new Customer1 { CustomerId = 2, Name = "Customer2" },
                new Customer1 { CustomerId = 3, Name = "Customer3" }
            };

            // Establecer opciones de importación con CheckMergedCells habilitado
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                InsertRows = true,
                CheckMergedCells = true
            };

            // Importar datos
            worksheet.Cells.ImportCustomObjects(customers, 0, 0, options);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Verificar que las celdas combinadas se conservaron
            Cell mergedCell = worksheet.Cells["D4"];
            Console.WriteLine($"Merged cell value: {mergedCell.StringValue}");
            Console.WriteLine($"Is cell merged: {mergedCell.IsMerged}");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


