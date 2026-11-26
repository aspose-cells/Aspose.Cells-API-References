---
title: "PivotTable.ShowReportFilterPageByName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Mostrar todas las páginas de filtro de informe según el nombre de PivotFields; el PivotField debe estar ubicado en PageFields"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showreportfilterpagebyname/
---
## PivotTable.ShowReportFilterPageByName method

Muestra todas las páginas de filtro de informe según el nombre del PivotField, el PivotField debe estar ubicado en los PageFields.

```csharp
public void ShowReportFilterPageByName(string fieldName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldName | String | El nombre del PivotField |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            
            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Agregar campo de página
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Fruit");
            pivotTable.PageFields[0].Name = "FruitFilter";
            
            // Actualizar tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Mostrar páginas de filtro de informe por nombre
            pivotTable.ShowReportFilterPageByName("FruitFilter");
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowReportFilterPageByNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


