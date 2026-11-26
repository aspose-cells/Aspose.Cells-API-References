---
title: "Top10Filter.Criteria"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Top10Filter. El valor real de la celda en el rango que se utiliza para realizar la comparación de este filtro. Este es el valor en caché durante el proceso de actualización"
type: docs
url: /es/net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

El valor real de la celda en el rango que se utiliza para realizar la comparación de este filtro. Este es el valor en caché durante el proceso de actualización.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, ignore esta propiedad. Esta propiedad será eliminada 12 meses después, a partir de octubre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class Top10FilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].PutValue(20 - i);
            }
            
            worksheet.AutoFilter.Range = "A1:A20";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Corrección: Acceder a la propiedad Filter y convertir a Top10Filter
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


