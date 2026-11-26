---
title: "Cells.GroupColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Cells method. Agrupa columnas"
type: docs
url: /es/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Agrupa columnas.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | El índice de la primera columna a agrupar. |
| lastIndex | Int32 | El índice de la última columna a agrupar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agrupar columnas desde el índice 0 hasta 255
            cells.GroupColumns(0, 255);

            // Guarda el libro de trabajo
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Agrupa columnas.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | El índice de la primera columna a agrupar. |
| lastIndex | Int32 | El índice de la última columna a agrupar. |
| isHidden | Booleano | Especifica si las columnas agrupadas están ocultas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agrupar columnas 5 a 7 (3 columnas) y ocultarlas
            cells.GroupColumns(5, 7, true);

            // Guarda el libro de trabajo
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


