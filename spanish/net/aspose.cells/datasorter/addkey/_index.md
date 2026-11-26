---
title: "DataSorter.AddKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DataSorter method. Agrega el índice de columna ordenada y el orden de clasificación"
type: docs
url: /es/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Agrega el índice de columna ordenada y el orden de clasificación.

```csharp
public void AddKey(int key, SortOrder order)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | Int32 | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| orden | SortOrder | El orden de clasificación |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Agregar clave de ordenación para la columna B (índice 1) con orden ascendente
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Ordenar rango de datos (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Salida de valores ordenados
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### Ver también

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Agrega el índice de columna ordenado y el orden de clasificación con una lista de clasificación personalizada.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | Int32 | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| orden | SortOrder | El orden de clasificación. |
| customList | String | La lista de ordenación personalizada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo para ordenar
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Crear clasificador de datos y agregar clave de ordenación personalizada
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Ordenar los datos
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Agrega el índice de columna ordenado y el orden de clasificación con una lista de clasificación personalizada.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | Int32 | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| type | SortOnType | El tipo de valor ordenado. |
| orden | SortOrder | El orden de clasificación. |
| customList | Objeto | La lista de ordenación personalizada. |

### Observaciones

Si el tipo es `SortOnType.CellColor` o `SortOnType.FontColor`, la customList es Color.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Crear un clasificador de datos
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // Llamar a AddKey con los parámetros: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Definir el rango a ordenar
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Ordenar los datos
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Agrega el índice de columna ordenado y el orden de clasificación con una lista de clasificación personalizada.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | Int32 | El índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...) |
| orden | SortOrder | El orden de clasificación. |
| customList | String[] | La lista de ordenación personalizada. |

### Ver también

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


