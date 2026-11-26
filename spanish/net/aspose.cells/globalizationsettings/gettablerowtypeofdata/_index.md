---
title: "GlobalizationSettings.GetTableRowTypeOfData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre del tipo de filas de tabla que consisten en la región de datos de la tabla referenciada. El valor predeterminado es Data, por lo que en la fórmula Data representa la región de datos de la tabla"
type: docs
url: /es/net/aspose.cells/globalizationsettings/gettablerowtypeofdata/
---
## GlobalizationSettings.GetTableRowTypeOfData method

Obtiene el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. El predeterminado es "Data", por lo que en la fórmula "#Data" representa la región de datos de la tabla.

```csharp
public virtual string GetTableRowTypeOfData()
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

    public class CustomGlobalizationSettings1 : GlobalizationSettings
    {
        public override string GetTableRowTypeOfData()
        {
            return "MyData";
        }
    }

    public class GlobalizationSettingsMethodGetTableRowTypeOfDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(1.8);

                // Corregidos los parámetros de ListObjects.Add para usar la sobrecarga correcta
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.ShowHeaderRow = true;
                table.DisplayName = "ProductTable";
                table.ShowTotals = true;
                table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

                Cell formulaCell = worksheet.Cells["B5"];
                formulaCell.Formula = "=SUM(ProductTable[#MyData])";

                workbook.CalculateFormula();
                Console.WriteLine($"Total price calculated: {formulaCell.Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfData method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


