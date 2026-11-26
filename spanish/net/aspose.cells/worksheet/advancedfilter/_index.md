---
title: "Worksheet.AdvancedFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Filtra datos usando criterios complejos"
type: docs
url: /es/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Filtra datos usando criterios complejos.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isFilter | Booleano | Indica si se está filtrando la lista en el lugar. |
| listRange | String | El rango de la lista. |
| criteriaRange | String | El rango de criterios. |
| copyTo | String | El rango al que se copian los datos. |
| uniqueRecordOnly | Booleano | Solo muestra o copia filas únicas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para el filtrado
            // Encabezados
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // Criterios
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // Datos
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // Aplicar filtro avanzado (filtrar en el lugar, solo registros únicos)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // Guarda el libro de trabajo
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


