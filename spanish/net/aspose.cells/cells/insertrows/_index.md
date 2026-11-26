---
title: "Cells.InsertRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Inserta múltiples filas en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

Inserta varias filas en la hoja de cálculo.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |
| totalRows | Int32 | Número de filas a insertar. |
| updateReference | Booleano | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Insertar una fila en el índice 2 (se convertirá en la nueva fila 3)
            worksheet.Cells.InsertRows(2, 1, true);
            
            // Agregar datos a la fila insertada
            worksheet.Cells["A3"].PutValue("Inserted Data");
            
            // Guarda el libro de trabajo
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

Inserta varias filas en la hoja de cálculo.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |
| totalRows | Int32 | Número de filas a insertar. |
| opciones | InsertOptions | Opciones para la operación de inserción. |

### Ejemplos

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Insertar 3 filas en el índice de fila 5 con las opciones especificadas
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            workbook.Save("InsertRowsWithOptions.xlsx");
        }
    }
}
```

### Ver también

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

Inserta varias filas en la hoja de cálculo.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |
| totalRows | Int32 | Número de filas a insertar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar algunos datos de ejemplo
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Data1");
            cells["B2"].PutValue("Data2");
            cells["A3"].PutValue("Data3");
            cells["B3"].PutValue("Data4");

            // Insertar 2 filas en el índice de fila 2
            cells.InsertRows(2, 2);

            // Verificar que las filas insertadas estén vacías
            Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
            Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"

            // Guarda el libro de trabajo
            workbook.Save("InsertRowsDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


