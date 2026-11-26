---
title: "AutoFilter.Custom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Filtra una lista con un criterio personalizado"
type: docs
url: /es/net/aspose.cells/autofilter/custom/
---
## Custom(int, FilterOperatorType, object) {#custom}

Filtra una lista con un criterio personalizado.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| operatorType1 | FilterOperatorType | El tipo de operador del filtro |
| criteria1 | Objeto | El criterio personalizado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a la columna A (10 filas + encabezado)
            worksheet.Cells["A1"].PutValue("Numbers");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i); // A2-A11: 1-10
            }

            // Establecer rango de autofiltro (A1:A11)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Aplicar filtro personalizado: Números > 5
                worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterThan, 5);
                
                // Actualizar el filtro para aplicar los cambios
                worksheet.AutoFilter.Refresh();
                
                Console.WriteLine("Custom filter applied: Column 0 values > 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }
            
            // Guardar el libro de trabajo filtrado
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Custom(int, FilterOperatorType, object, bool, FilterOperatorType, object) {#custom_1}

Filtra una lista con criterios personalizados.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1, bool isAnd, 
    FilterOperatorType operatorType2, object criteria2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| operatorType1 | FilterOperatorType | El tipo de operador del filtro |
| criteria1 | Objeto | El criterio personalizado |
| isAnd | Booleano |  |
| operatorType2 | FilterOperatorType | El tipo de operador del filtro |
| criteria2 | Objeto | El criterio personalizado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellene datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product ID");
            worksheet.Cells["A2"].PutValue(85);
            worksheet.Cells["A3"].PutValue(42);
            worksheet.Cells["A4"].PutValue(65);
            worksheet.Cells["A5"].PutValue(95);
            worksheet.Cells["A6"].PutValue(30);
            worksheet.Cells["A7"].PutValue(75);

            // Establecer rango de autofiltro (A1:A7)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 0); // Start row: 0 (A1), strartt column: 0 (A), end Column: 0 (A)

            try
            {
                // Aplicar filtro personalizado: Mayor o igual a 50 Y Menor o igual a 100
                autoFilter.Custom(
                    0, // Field index (column A)
                    FilterOperatorType.GreaterOrEqual,
                    50, // First criteria
                    true, // AND combination
                    FilterOperatorType.LessOrEqual,
                    100 // Second criteria
                );

                Console.WriteLine("Custom filter applied successfully with parameters: " +
                    "(Int32, FilterOperatorType, Object, Boolean, FilterOperatorType, Object)");

                // Actualizar filtros y guardar resultados
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }

            // Guardar el libro de trabajo filtrado
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


