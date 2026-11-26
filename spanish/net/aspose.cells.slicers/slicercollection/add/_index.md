---
title: "SlicerCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SlicerCollection. Añade un nuevo Slicer usando PivotTable como fuente de datos"
type: docs
url: /es/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Agregar un nuevo Slicer usando PivotTable como origen de datos

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| destCellName | String | La celda en la esquina superior izquierda del rango del Slicer. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // Agregar slicer
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Agregar un nuevo Slicer usando PivotTable como origen de datos

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango del Slicer. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango del Slicer. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Fruit");
            cells["B1"].PutValue("Quantity");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(50);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(30);

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar slicer
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivotTable, 20, 12, "fruit");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Agregar un nuevo Slicer usando PivotTable como origen de datos

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango del Slicer. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango del Slicer. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Agregar tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Añadir slicer para la tabla dinámica
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Agregar un nuevo Slicer usando PivotTable como origen de datos

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| destCellName | String | La celda en la esquina superior izquierda del rango del Slicer. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Agregar slicer
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Agregar un nuevo Slicer usando PivotTable como origen de datos

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango del Slicer. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango del Slicer. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Agregar campos de tabla dinámica
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar slicer
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Guarda el libro de trabajo
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Agregar un nuevo Slicer usando PivotTable como origen de datos

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | Objeto PivotTable |
| destCellName | String | La celda en la esquina superior izquierda del rango del Slicer. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // Agregar slicer
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // Guarda el libro de trabajo
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Agrega un nuevo Slicer usando ListObjet como fuente de datos

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tabla | ListObject | Objeto ListObject |
| índice | Int32 | El índice de ListColumn en ListObject.ListColumns |
| destCellName | String | La celda en la esquina superior izquierda del rango del Slicer. |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de muestra y objeto de lista
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Añadir slicer para el objeto de lista - nota: Slicers.Add devuelve un índice int
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Guarda el libro de trabajo
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Agrega un nuevo Slicer usando ListObjet como fuente de datos

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tabla | ListObject | Objeto ListObject |
| listColumn | ListColumn | El ListColumn en ListObject.ListColumns |
| destCellName | String | La celda en la esquina superior izquierda del rango del Slicer. |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");

            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, table.ListColumns[1], "I38");

            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells.SetColumnWidth(1, 20);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Agrega un nuevo Slicer usando ListObjet como fuente de datos

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tabla | ListObject | Objeto ListObject |
| listColumn | ListColumn | El ListColumn en ListObject.ListColumns |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango del Slicer. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango del Slicer. |

### Valor de retorno

El nuevo índice de Slicer añadido

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnInt32Int32Demo
    {
        public static void Run()
        {
            // Crear libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Añadir datos de muestra para la tabla
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue("CatA");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue("CatB");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue("CatA");
            
            // Crear rango de tabla
            int endRow = 4;
            string startCell = "A1";
            string endCell = $"B{endRow}";
            
            // Añadir tabla a la hoja de cálculo usando la sobrecarga correcta
            int tableIndex = sheet.ListObjects.Add(startCell, endCell, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Añadir slicer para la columna Category en la posición (fila 6, columna 1)
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(table, table.ListColumns[1], 6, 1);
            
            // Guardar resultado
            workbook.Save("SlicerOutput.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


