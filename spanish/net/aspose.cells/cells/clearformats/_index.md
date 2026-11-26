---
title: "Cells.ClearFormats"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina el formato de un rango"
type: docs
url: /es/net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Borra el formato de un rango.

```csharp
public void ClearFormats(CellArea range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | CellArea | Rango a eliminar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos de muestra con formato
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // Aplicar formato a las celdas
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            
            for (int row = formatArea.StartRow; row <= formatArea.EndRow; row++)
            {
                for (int col = formatArea.StartColumn; col <= formatArea.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Formatted {row},{col}");
                    cells[row, col].SetStyle(style);
                }
            }

            // Definir área de borrado
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // Eliminar formatos de la celda central
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // Actualizar el valor de la celda borrada para mostrar el efecto
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // Guardar resultado
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearFormats(int, int, int, int) {#clearformats_1}

Borra el formato de un rango.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| startColumn | Int32 | Índice de columna inicial. |
| endRow | Int32 | Índice de fila final. |
| endColumn | Int32 | Índice de columna final. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearFormatsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aplicar estilos a algunas celdas
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            cells[0, 0].SetStyle(style);
            cells[0, 10].SetStyle(style);
            cells[10, 0].SetStyle(style);
            cells[10, 10].SetStyle(style);

            // Eliminar formatos de un rango específico (filas 5-15, columnas 5-15)
            cells.ClearFormats(5, 5, 15, 15);

            // Guarda el libro de trabajo
            workbook.Save("ClearedFormats.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


