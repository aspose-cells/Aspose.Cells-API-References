---
title: "Cell.GetTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene la tabla que contiene esta celda"
type: docs
url: /es/net/aspose.cells/cell/gettable/
---
## Cell.GetTable method

Obtiene la tabla que contiene esta celda.

```csharp
public ListObject GetTable()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellMethodGetTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Cree una tabla con encabezados y datos
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Cree un ListObject (tabla) a partir del rango de datos
            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Demuestre el método GetTable
            Cell cellInTable = cells["B2"];
            ListObject resultTable = cellInTable.GetTable();
            
            Console.WriteLine("Table found: " + (resultTable != null));
            Console.WriteLine("Table range: " + resultTable.StartRow + "," + resultTable.StartColumn + 
                            " to " + resultTable.EndRow + "," + resultTable.EndColumn);
        }
    }
}
```

### Ver también

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


