---
title: "Cells.CopyColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Copia datos y formatos de una columna completa"
type: docs
url: /es/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Copia los datos y formatos de una columna completa.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | Int32 | Índice de la columna de origen. |
| destinationColumnIndex | Int32 | Índice de la columna de destino. |
| columnNumber | Int32 | El número de columna copiada. |
| pasteOptions | PasteOptions | las opciones de pegado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Crear otro libro de trabajo como destino
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // Copiar columnas solo con formato
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // Guarda el libro de trabajo
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

Copia los datos y formatos de columnas completas.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | Int32 | Índice de la columna de origen. |
| destinationColumnIndex | Int32 | Índice de la columna de destino. |
| columnNumber | Int32 | El número de columna copiada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo a las columnas
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // Copiar columnas del índice de columna 1 (B) al índice de columna 3 (D), copiar 1 columna
            cells.CopyColumns(cells, 1, 3, 1);

            // Guarda el libro de trabajo
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Copia los datos y formatos de todas las columnas.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | Int32 | Índice de la columna de origen. |
| sourceTotalColumns | Int32 | El número de columnas de origen. |
| destinationColumnIndex | Int32 | Índice de la columna de destino. |
| destinationTotalColumns | Int32 | El número de columnas de destino. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar columnas de origen (columnas 0 y 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // Copiar 2 columnas del índice 0 al índice de destino 3, insertando 2 columnas
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // Verificar la copia comprobando las columnas de destino (3 y 4)
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


