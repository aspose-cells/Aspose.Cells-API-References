---
title: "Cells.InsertRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento"
type: docs
url: /es/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| área | CellArea | Desplazar área. |
| shiftNumber | Int32 | Número de filas o columnas a insertar. |
| shiftType | ShiftType | Opción de desplazar celdas. |
| updateReference | Booleano | Indica si se actualizan referencias en otras hojas de cálculo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos de muestra
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // Definir el área a insertar (filas 2-3, columna A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // Insertar rango desplazando celdas a la derecha y actualizar referencias
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // Verificar la operación comprobando los valores
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| área | CellArea | Desplazar área. |
| shiftType | ShiftType | Opción de desplazar celdas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Rellenar algunos datos de muestra
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // Definir el área de celdas a insertar
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // Insertar rango y desplazar celdas hacia abajo
            cells.InsertRange(area, ShiftType.Down);

            // Guarda el libro de trabajo
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| área | CellArea | Desplazar área. |
| shiftNumber | Int32 | Número de filas o columnas a insertar. |
| shiftType | ShiftType | Opción de desplazar celdas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // Definir el área de celdas a insertar (celda única B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // Insertar rango desplazando celdas a la derecha
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // Guarda el libro de trabajo
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


