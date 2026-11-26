---
title: "SettableGlobalizationSettings.GetTableRowTypeOfData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. El valor predeterminado es Data, por lo que en la fórmula Data representa la región de datos de la tabla"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/
---
## SettableGlobalizationSettings.GetTableRowTypeOfData method

Obtiene el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. El predeterminado es "Data", por lo que en la fórmula "#Data" representa la región de datos de la tabla.

```csharp
public override string GetTableRowTypeOfData()
```

### Valor de retorno

el nombre de tipo de las filas de tabla

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
                settings.SetTableRowTypeOfData("CustomData");
                string rowType = settings.GetTableRowTypeOfData();
                Console.WriteLine($"TableRowTypeOfData: {rowType}");

                workbook.Settings.GlobalizationSettings = settings;

                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["B2"].PutValue(5.5);
                worksheet.Cells["B3"].PutValue(3.8);

                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "Inventory"; // Changed from Name to DisplayName
                
                worksheet.Cells["B4"].Formula = "=SUM(Inventory[#CustomData][Price])";
                
                workbook.CalculateFormula();
                Console.WriteLine($"Total price: {worksheet.Cells["B4"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


