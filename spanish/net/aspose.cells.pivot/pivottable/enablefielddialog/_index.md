---
title: "PivotTable.EnableFieldDialog"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si el cuadro de diálogo de campo de la PivotTable está disponible cuando el usuario hace doble clic en el campo de la PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/enablefielddialog/
---
## PivotTable.EnableFieldDialog property

Indica si el cuadro de diálogo del campo de PivotTable está disponible cuando el usuario hace doble clic en el campo de PivotTable.

```csharp
public bool EnableFieldDialog { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableFieldDialogDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Demostrar la propiedad EnableFieldDialog
            pivotTable.EnableFieldDialog = true;
            Console.WriteLine("EnableFieldDialog set to: " + pivotTable.EnableFieldDialog);

            // Cambiar la propiedad y verificar
            pivotTable.EnableFieldDialog = false;
            Console.WriteLine("EnableFieldDialog changed to: " + pivotTable.EnableFieldDialog);

            // Guarda el libro de trabajo
            workbook.Save("PivotTable_EnableFieldDialog_Example.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


