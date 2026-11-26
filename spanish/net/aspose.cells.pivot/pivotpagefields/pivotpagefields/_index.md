---
title: "PivotPageFields.PivotPageFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de PivotPageFields. Representa los elementos del campo de página dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Representa los elementos de campo de página pivot.

```csharp
public PivotPageFields()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // Crear campos de página dinámica usando el constructor
            PivotPageFields pageFields = new PivotPageFields();
            
            // Agregar campos de página
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // Agregar identificación
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // Agregar tabla dinámica con los parámetros correctos
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // Guarda el libro de trabajo
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


