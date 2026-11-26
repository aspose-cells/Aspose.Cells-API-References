---
title: "ListObjectCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListObjectCollection. Añade un ListObject a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Agrega un ListObject a la hoja de cálculo.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La fila de inicio del rango de lista. |
| startColumn | Int32 | La fila de inicio del rango de lista. |
| endRow | Int32 | La fila de inicio del rango de lista. |
| endColumn | Int32 | La fila de inicio del rango de lista. |
| hasHeaders | Booleano | Indica si el rango tiene encabezados. |

### Valor de retorno

El índice del nuevo ListObject

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos en un rango
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // Agregar ListObject usando el método Add con parámetros Int32
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Habilitar totales y establecer fórmula para una columna
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // Guarda el libro de trabajo
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Agrega un ListObject a la hoja de cálculo.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startCell | String | La celda inicial del rango de la lista. |
| endCell | String | La celda final del rango de la lista. |
| hasHeaders | Booleano | Indica si el rango tiene encabezados. |

### Valor de retorno

El índice del nuevo ListObject

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellene datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // Agregar objeto de lista usando referencias de rango de cadena
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Ver también

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


