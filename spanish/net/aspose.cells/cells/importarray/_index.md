---
title: "Cells.ImportArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells."
type: docs
url: /es/net/aspose.cells/cells/importarray/
---
## ImportArray(string[], int, int) {#importarray_4}

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn)
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(string[], int, int, bool) {#importarray_5}

Importa una matriz de string a una hoja de cálculo.

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringArray | String[] | Matriz de String. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| isVertical | Booleano | Especifica si se importan los datos verticalmente u horizontalmente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara los datos de la matriz de string
            string[] fruitArray = new string[] { "Apple", "Banana", "Cherry", "Date", "Elderberry" };

            try
            {
                // Llama a ImportArray con los parámetros: (String[], Int32, Int32, Boolean)
                // Comienza la importación en la fila 2 (tercera fila), columna 1 (columna B), verticalmente
                worksheet.Cells.ImportArray(fruitArray, 2, 1, true);

                Console.WriteLine("Imported string array vertically starting from cell B3:");
                foreach (string fruit in fruitArray)
                {
                    Console.WriteLine(fruit);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("CellsMethodImportArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int) {#importarray_2}

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn)
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int, bool) {#importarray_3}

Importa una matriz de integer a una hoja de cálculo.

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intArray | Int32[] | Matriz de Integer. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| isVertical | Booleano | Especifica si se importan los datos verticalmente u horizontalmente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithInt32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara los datos de la matriz de Int32
            int[] data = new int[] { 1, 2, 3, 4, 5 };

            try
            {
                // Llama a ImportArray con los parámetros: (Int32[], firstRow=2, firstColumn=1, isVertical=true)
                worksheet.Cells.ImportArray(data, 2, 1, true);

                Console.WriteLine("Imported array vertically starting from cell B3:");
                for (int i = 0; i < data.Length; i++)
                {
                    Console.WriteLine($"Cell B{3 + i}: {worksheet.Cells[2 + i, 1].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("CellsMethodImportArrayWithInt32Int32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int) {#importarray}

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn)
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int, bool) {#importarray_1}

Importa una matriz de double a una hoja de cálculo.

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| doubleArray | Double[] | Matriz de Double. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| isVertical | Booleano | Especifica si se importan los datos verticalmente u horizontalmente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithDoubleInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Prepara datos de muestra de la matriz de double
            double[] dataArray = new double[] { 1.23, 4.56, 7.89, 10.11, 12.13 };
            const int targetRow = 2;    // 0-based row index (3rd row)
            const int targetColumn = 1; // 0-based column index (2nd column)
            const bool isVertical = true;

            try
            {
                // Obtén la colección de celdas y llama a ImportArray
                Cells cells = worksheet.Cells;
                cells.ImportArray(dataArray, targetRow, targetColumn, isVertical);
                
                Console.WriteLine($"Imported {dataArray.Length} double values starting at row {targetRow + 1}, column {targetColumn + 1}");
                Console.WriteLine($"Data orientation: {(isVertical ? "Vertical" : "Horizontal")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("CellsImportArrayDoubleVerticalDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


