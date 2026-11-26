---
title: "PivotFilter.GetNumberValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilter. Obtiene los valores del filtro numérico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/getnumbervalues/
---
## PivotFilter.GetNumberValues method

Obtiene los valores del filtro numérico.

```csharp
public double[] GetNumberValues()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetNumberValuesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 5;
            sheet.Cells["B3"].Value = 3;
            sheet.Cells["B4"].Value = 2;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Aplicar filtro de valor
            pivotTable.RowFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 4, 0);
            
            // Obtener y mostrar los valores del filtro
            PivotFilter filter = pivotTable.RowFields[0].GetFilters()[0];
            double[] numberValues = filter.GetNumberValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Number Values: " + string.Join(", ", numberValues));
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


