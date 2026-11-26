---
title: "Cells.InsertColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Inserta una nueva columna en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Inserta una nueva columna en la hoja de cálculo.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de columna. |
| updateReference | Booleano | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Rellena algunos datos de ejemplo en la columna 0
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // Inserta una nueva columna en el índice 1 y desplaza las columnas a la derecha
            cells.InsertColumn(1, true);

            // Copia datos de la columna 0 a la nueva columna 1
            cells.CopyColumn(cells, 0, 1);

            // Guarda el libro de trabajo
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Inserta una nueva columna en la hoja de cálculo.

```csharp
public void InsertColumn(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtén la colección de celdas
            Cells cells = sheet.Cells;
            
            // Inserta datos en las celdas para demostración
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Inserta una nueva columna en el índice 1 (se convertirá en la nueva columna B)
            cells.InsertColumn(1);
            
            // Verifica insertando datos en la nueva columna
            cells["B1"].PutValue("New Column");
            
            // Guarda el libro de trabajo
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


