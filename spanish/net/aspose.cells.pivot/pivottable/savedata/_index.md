---
title: "PivotTable.SaveData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si los datos del informe de la tabla dinámica se guardan con el libro de trabajo"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/savedata/
---
## PivotTable.SaveData property

Indica si los datos del informe de la tabla dinámica se guardan con el libro de trabajo.

```csharp
public bool SaveData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySaveDataDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Demostrar la propiedad SaveData
            Console.WriteLine("SaveData before setting: " + pivotTable.SaveData);
            pivotTable.SaveData = false; // Disable saving pivot data with file
            Console.WriteLine("SaveData after setting: " + pivotTable.SaveData);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTable_SaveData_Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


