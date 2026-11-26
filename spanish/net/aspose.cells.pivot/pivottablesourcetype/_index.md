---
title: "Enumeración PivotTableSourceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Pivot.PivotTableSourceType enum. Representa el tipo de origen de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

Representa el tipo de origen de datos de la tabla dinámica.

```csharp
public enum PivotTableSourceType : byte
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Sheet | `1` | Especifica que los datos de origen son un rango. |
| External | `2` | Especifica que se utilizan datos de origen externos. |
| Consolidation | `4` | Especifica que se utilizan varios rangos de consolidación como datos de origen. |
| Scenario | `8` | Los datos de origen se rellenan a partir de una estructura interna temporal. |
| Unknown | `9` | Origen de datos desconocido. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar datos de ejemplo a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Crear una colección de tablas dinámicas
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Agregar una tabla dinámica usando Sheet como tipo de origen
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Mostrar el tipo de origen
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Demostrar diferentes tipos de origen
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Guarda el libro de trabajo
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


