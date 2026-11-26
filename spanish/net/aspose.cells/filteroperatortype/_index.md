---
title: "Enum FilterOperatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.FilterOperatorType. Tipo de operador de filtro personalizado"
type: docs
url: /es/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Tipo de operador de filtro personalizado.

```csharp
public enum FilterOperatorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| LessOrEqual | `0` | Representa el operador Menor o Igual. |
| LessThan | `1` | Representa el operador Menor que. |
| Equal | `2` | Representa el operador Igual. |
| GreaterThan | `3` | Representa el operador Mayor que. |
| NotEqual | `4` | Representa el operador No Igual. |
| GreaterOrEqual | `5` | Representa el operador GreaterOrEqual. |
| None | `6` | Representa sin comparación. |
| BeginsWith | `7` | Comienza con el texto. |
| EndsWith | `8` | Termina con el texto. |
| Contains | `9` | Contiene el texto. |
| NotContains | `10` | No contiene el texto. |
| NotBeginsWith | `11` | No comienza con el texto. |
| NotEndsWith | `12` | No termina con el texto. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // Establecer rango de filtro automático
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Aplicar filtro personalizado para mostrar nombres que comienzan con "Bo"
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // Actualizar el filtro
            worksheet.AutoFilter.Refresh();
            
            // Guarda el libro de trabajo
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


