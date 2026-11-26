---
title: "TimelineCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TimelineCollection. Añade una nueva Línea de tiempo usando PivotTable como fuente de datos"
type: docs
url: /es/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Agregar una nueva Línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de la Timeline. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de la Timeline. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de agregar Timeline

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // Agregar timeline conectado a la tabla dinámica
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // Guardar el libro de trabajo
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Agregar una nueva Línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| destCellName | String | El nombre de la celda en la esquina superior izquierda del rango de Timeline. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de agregar Timeline

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // Agregar tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Agregar timeline conectado a la tabla dinámica
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // Guarda el libro de trabajo
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Agregar una nueva Línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de la Timeline. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de la Timeline. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de agregar Timeline

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Agregar tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar control de timeline
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Agregar una nueva Línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| destCellName | String | El nombre de la celda en la esquina superior izquierda del rango de Timeline. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de agregar Timeline

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Encontrar el índice del campo base para el campo "Date"
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // Agregar timeline usando el índice encontrado
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // Guardar el resultado
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Agregar una nueva Línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de la Timeline. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de la Timeline. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de agregar Timeline

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // Agregar campos de tabla dinámica
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // Agregar timeline usando la tabla dinámica
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // Guarda el libro de trabajo
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Agregar una nueva Línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| destCellName | String | El nombre de la celda en la esquina superior izquierda del rango de Timeline. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de agregar Timeline

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Agregar timeline usando la tabla dinámica como fuente de datos
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


