---
title: "Protection.AllowUsingPivotTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Protection property. Representa si el usuario tiene permiso para manipular tablas dinámicas en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Representa si se permite al usuario manipular tablas dinámicas en una hoja de cálculo protegida.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowUsingPivotTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Habilitar la protección de la hoja de cálculo
            Protection protection = worksheet.Protection;
            protection.AllowUsingPivotTable = true;
            worksheet.Protect(ProtectionType.All);

            // Verifique la configuración
            Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);

            // Crea una tabla dinámica para demostrar la funcionalidad
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Crea una tabla dinámica con los parámetros correctos
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Guarda el libro de trabajo
            workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


