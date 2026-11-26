---
title: "Cell.GetPrecedents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene todas las referencias que aparecen en la fórmula de esta celda"
type: docs
url: /es/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

Obtiene todas las referencias que aparecen en la fórmula de esta celda.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### Valor de retorno

Colección de todas las referencias que aparecen en la fórmula de esta celda.

### Observaciones

Devuelve null si esta no es una celda de fórmula. Todas las referencias que aparecen en la fórmula de esta celda se devolverán sin importar si están referenciadas o no durante el cálculo. Por ejemplo, aunque la celda A2 en la fórmula "=IF(TRUE,A1,A2)" no se use durante el cálculo, aún se considera como precedentes de la fórmula. Para obtener solo aquellas referencias que influyen en el cálculo, utilice [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Establecer fórmula con precedentes
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // Obtener todas las referencias precedentes
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Mostrar cada referencia precedente
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                Console.WriteLine(sb.ToString());
            }
        }
    }
}
```

### Ver también

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


