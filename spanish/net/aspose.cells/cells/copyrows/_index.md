---
title: "Cells.CopyRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Copia datos y formatos de algunas filas completas"
type: docs
url: /es/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Copia los datos y formatos de algunas filas completas.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | Int32 | Índice de fila de origen. |
| destinationRowIndex | Int32 | Índice de fila de destino. |
| rowNumber | Int32 | El número de fila copiada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // Añade algunos datos de ejemplo al libro de origen
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // Obtén las celdas de ambos libros
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // Copia todas las filas del origen al destino comenzando en la fila 0 del destino
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // Guardar el resultado
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Copia los datos y formatos de algunas filas completas.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | Int32 | Índice de fila de origen. |
| destinationRowIndex | Int32 | Índice de fila de destino. |
| rowNumber | Int32 | El número de fila copiada. |
| copyOptions | CopyOptions | Las opciones de copia. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade algunos datos de ejemplo e hipervínculos
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Inserta una fila en blanco en la fila 5
            worksheet.Cells.InsertRows(5, 1);

            // Copiar fila 4 a fila 5 sin CopyOptions
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // Restablecer la hoja de cálculo
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Insertar una fila en blanco en la fila 5 nuevamente
            worksheet.Cells.InsertRows(5, 1);

            // Copiar fila 4 a fila 5 con CopyOptions
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Ver también

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Copia los datos y formatos de algunas filas completas.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells0 | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | Int32 | Índice de fila de origen. |
| destinationRowIndex | Int32 | Índice de fila de destino. |
| rowNumber | Int32 | El número de fila copiada. |
| copyOptions | CopyOptions | Las opciones de copia. |
| pasteOptions | PasteOptions | las opciones de pegado. |

### Ver también

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


