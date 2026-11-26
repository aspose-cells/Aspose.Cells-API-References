---
title: "WorksheetCollection.GetRangeByName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Obtiene el objeto Range por nombre predefinido"
type: docs
url: /es/net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Obtiene el objeto Range por nombre predefinido.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeName | String | Nombre del rango. |

### Valor de retorno

Objeto Range.

Devuelve null si el rango con nombre no existe.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetRangeByNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Crear un rango con nombre
            worksheet.Cells.CreateRange("A1:B2").Name = "FruitData";
            
            // Obtener el rango con nombre usando GetRangeByName
            Aspose.Cells.Range namedRange = workbook.Worksheets.GetRangeByName("FruitData");
            
            // Mostrar información del rango si se encuentra
            if (namedRange != null)
            {
                Console.WriteLine("Range found: " + namedRange.Address);
                Console.WriteLine("First cell value: " + namedRange[0, 0].StringValue);
            }
            else
            {
                Console.WriteLine("Range not found");
            }
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Obtiene [`Range`](../../range/) por nombre predefinido o nombre de tabla

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeName | String | Nombre del rango o nombre de tabla. |
| currentSheetIndex | Int32 | El índice de la hoja. -1 representa global. |
| includeTable | Booleano | Indica si se están verificando todas las tablas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetRangeByNameWithStringInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango con nombre
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1", "C3");
            namedRange.Name = "TestRange";
            
            // Agregar algunos datos al rango
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            try
            {
                // Llamar a GetRangeByName con los parámetros (String, Int32, Boolean)
                Aspose.Cells.Range retrievedRange = workbook.Worksheets.GetRangeByName("TestRange", 0, true);
                
                Console.WriteLine("Method executed successfully with parameters (String, Int32, Boolean)");
                Console.WriteLine($"Retrieved range address: {retrievedRange.Address}");
                Console.WriteLine($"Range contains {retrievedRange.RowCount} rows and {retrievedRange.ColumnCount} columns");
                
                // Mostrar valores del rango
                Console.WriteLine("Range values:");
                foreach (Cell cell in retrievedRange)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRangeByName method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("WorksheetCollectionMethodGetRangeByNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


