---
title: "Workbook.Replace"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Reemplaza el valor de una celda con una nueva cadena"
type: docs
url: /es/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Reemplaza el valor de una celda con una cadena nueva.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValue | String | Valor de cadena a reemplazar |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // Reemplazar todas las ocurrencias de "Apple" con "Mango"
            workbook.Replace("Apple", "Mango");
            
            // Guarda el libro de trabajo
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Reemplaza el valor de una celda con un entero nuevo.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValue | Int32 | Valor entero a reemplazar |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja y agregar algunos datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // Reemplazar todas las ocurrencias de "OriginalValue" con el entero 100
            workbook.Replace("OriginalValue", 100);
            
            // Guarda el libro de trabajo
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Reemplaza el valor de una celda con un double nuevo.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValue | Double | Valor doble a reemplazar |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Colocar algunos datos de ejemplo en las celdas
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Reemplazar texto con valor doble
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Reemplaza el valor de una celda con una nueva matriz de string.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValues | String[] | Arreglo de String a reemplazar |
| isVertical | Booleano | True - Vertical, False - Horizontal |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a las celdas
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Definir nuevos valores para reemplazar
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // Reemplazar todas las ocurrencias de "AnOldValue" con los nuevos valores
            workbook.Replace("AnOldValue", newValues, true);
            
            // Guarda el libro de trabajo
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Reemplaza los valores de las celdas con una matriz de integer.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValues | Int32[] | Arreglo de Integer a reemplazar |
| isVertical | Booleano | True - Vertical, False - Horizontal |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a las celdas
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // Definir valores de reemplazo
            int[] newValues = new int[] { 1, 2, 3 };
            
            // Reemplazar "OldValue" con el arreglo de enteros
            workbook.Replace("OldValue", newValues, true);
            
            // Guarda el libro de trabajo
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Reemplaza los valores de las celdas con una matriz de double.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValues | Double[] | Arreglo de Double a reemplazar |
| isVertical | Booleano | True - Vertical, False - Horizontal |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Definir valores de reemplazo
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // Reemplazar todas las ocurrencias de "AnOldValue" con los nuevos valores
            workbook.Replace("AnOldValue", newValues, true);
            
            // Guarda el libro de trabajo
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Reemplaza los valores de las celdas con datos de una DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| insertTable | DataTable | DataTable a reemplazar |

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDataTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear un DataTable de ejemplo
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // Agregar datos de ejemplo al DataTable
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // Agregar algún texto a la hoja de cálculo que será reemplazado
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // Reemplazar el texto con DataTable
            workbook.Replace("CustomerData", dataTable);
            
            // Guarda el libro de trabajo
            workbook.Save("Output.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Reemplaza los valores de las celdas con datos nuevos.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| boolValue | Booleano | El valor booleano a ser reemplazado. |
| newValue | Objeto | Nuevo valor. Puede ser string, integer, double o valor DateTime. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellene algunas celdas con valores booleanos
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Llame al método Replace para reemplazar todos los valores 'true' con "REPLACED"
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Muestra los resultados
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Reemplaza los valores de las celdas con datos nuevos.

```csharp
public int Replace(int intValue, object newValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intValue | Int32 | El valor entero a ser reemplazado. |
| newValue | Objeto | Nuevo valor. Puede ser string, integer, double o valor DateTime. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellene algunas celdas con valores integer a ser reemplazados
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Llame al método Replace con los parámetros (Int32, Object)
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Muestre el contenido de la hoja de cálculo después del reemplazo
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Reemplaza el valor de una celda con una cadena nueva.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValue | String | Valor de cadena a reemplazar |
| opciones | ReplaceOptions | Las opciones de reemplazo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false
            };

            int replacedCount = workbook.Replace("Hello", "Hi", options);

            Console.WriteLine($"Replacements made: {replacedCount}");
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


