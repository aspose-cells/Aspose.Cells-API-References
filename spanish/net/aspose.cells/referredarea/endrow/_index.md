---
title: "ReferredArea.EndRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. La fila final del área"
type: docs
url: /es/net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

La fila final del área.

```csharp
public int EndRow { get; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyEndRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Establecer fórmula con múltiples referencias
            cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
            
            // Obtener todas las áreas precedentes
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Procesar cada referencia
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                
                // Demostrar el uso de EndRow para referencias de rango
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                
                Console.WriteLine(sb.ToString());
            }
            
            workbook.Save("ReferredAreaExample.xlsx");
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


