---
title: "PivotTable.RefreshDataOnOpeningFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si se actualizan los datos al abrir el archivo"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/refreshdataonopeningfile/
---
## PivotTable.RefreshDataOnOpeningFile property

Indica si se actualizan los datos al abrir el archivo.

```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDataOnOpeningFileDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Banana";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Orange";
            cells["B4"].Value = 3000;

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Establecer la propiedad RefreshDataOnOpeningFile
            pivotTable.RefreshDataOnOpeningFile = false;

            // Guarda el libro de trabajo
            workbook.Save("PivotTableRefreshDataOnOpeningFileDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


