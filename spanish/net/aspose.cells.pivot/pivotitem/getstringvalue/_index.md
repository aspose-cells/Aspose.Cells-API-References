---
title: "PivotItem.GetStringValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotItem. Obtiene el valor de cadena del elemento pivot. Si el valor es nulo, devolverá"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Obtiene el valor de cadena del elemento pivot. Si el valor es nulo, devolverá ""

```csharp
public string GetStringValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceda a la primera hoja de cálculo y tabla dinámica
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Obtenga el primer campo de fila y sus elementos pivot
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // Demuestre el método GetStringValue()
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // Guardar el libro de trabajo modificado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


