---
title: "Clase CellsDataTableFactory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CellsDataTableFactory. Utilidad para crear ICellsDataTable a partir de objetos personalizados para la conveniencia del usuario"
type: docs
url: /es/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Utilidad para crear ICellsDataTable a partir de objetos personalizados para la comodidad del usuario.

```csharp
public class CellsDataTableFactory
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Crea ICellsDataTable a partir de la colección proporcionada. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Crea ICellsDataTable a partir de la secuencia dada de valores double. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Crea ICellsDataTable a partir de la secuencia dada de valores double. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | Crea ICellsDataTable a partir de la colección proporcionada. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Crea ICellsDataTable a partir de la secuencia dada de valores enteros. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Crea ICellsDataTable a partir de la secuencia dada de valores enteros. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | Crea ICellsDataTable a partir de la secuencia dada de objetos. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | Crea ICellsDataTable a partir de la secuencia dada de objetos. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | Crea un ICellsDataTable a partir de una secuencia dada de objetos. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Obtener la instancia de CellsDataTableFactory del libro de trabajo
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Crear una instancia de ICellsDataTable a partir de la lista de datos personalizada
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importar la tabla de datos en la hoja de cálculo comenzando en la celda A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Guarda el libro de trabajo
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Clase de datos personalizada
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


