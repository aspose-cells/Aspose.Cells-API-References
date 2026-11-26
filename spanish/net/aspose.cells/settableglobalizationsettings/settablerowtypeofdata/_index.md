---
title: "SettableGlobalizationSettings.SetTableRowTypeOfData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de tipo de las filas de tabla que consisten en la región de datos de la tabla referenciada"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/settablerowtypeofdata/
---
## SettableGlobalizationSettings.SetTableRowTypeOfData method

Establece el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada.

```csharp
public void SetTableRowTypeOfData(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | el nombre de tipo de las filas de tabla |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una tabla
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

            // Crear configuraciones de globalización
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Establecer nombre personalizado para filas de datos en la tabla
                settings.SetTableRowTypeOfData("MyDataRegion");
                
                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table row type of data set to: MyDataRegion");
                Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


