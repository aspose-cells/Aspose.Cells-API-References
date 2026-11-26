---
title: "Cells.InsertCutCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Insertar rango recortado"
type: docs
url: /es/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Insertar rango recortado.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cutRange | Rango | El rango recortado. |
| fila | Int32 | La fila. |
| columna | Int32 | La columna. |
| shiftType | ShiftType | Indica cómo desplazar otros objetos del rango objetivo al insertar el rango recortado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y sus celdas
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // Agregar algunos datos a las celdas de origen
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // Crear una segunda hoja de cálculo como destino
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // Agregar algunos datos iniciales al destino
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // Crear un rango para recortar (A1:B2 de la hoja de origen)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // Insertar las celdas recortadas en B2 en la hoja de destino, desplazando las celdas hacia abajo
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // Guarda el libro de trabajo
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


