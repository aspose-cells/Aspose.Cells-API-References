---
title: "Workbook.CellsDataTableFactory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene la fábrica para crear ICellsDataTable a partir de objetos personalizados"
type: docs
url: /es/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Obtiene la fábrica para crear ICellsDataTable a partir de objetos personalizados

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }

    public class WorkbookPropertyCellsDataTableFactoryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Obtener CellsDataTableFactory de la propiedad del libro de trabajo
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Crear tabla de datos a partir de una lista
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importar datos a la hoja de cálculo
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Guardar salidas
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


