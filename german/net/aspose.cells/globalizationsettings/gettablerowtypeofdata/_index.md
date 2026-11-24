---
title: "GlobalizationSettings.GetTableRowTypeOfData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Typnamen der Tabellenzeilen zurück, die aus dem Datenbereich der referenzierten Tabelle bestehen. Standard ist Data, sodass in der Formel Data den Datenbereich der Tabelle darstellt."
type: docs
url: /de/net/aspose.cells/globalizationsettings/gettablerowtypeofdata/
---
## GlobalizationSettings.GetTableRowTypeOfData method

Gibt den Typnamen der Tabellenzeilen zurück, die den Datenbereich der referenzierten Tabelle umfassen. Standard ist "Data", sodass in der Formel "#Data" den Datenbereich der Tabelle darstellt.

```csharp
public virtual string GetTableRowTypeOfData()
```

### Rückgabewert

der Typname von Tabellenzeilen

### Beispiele

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

                // ListObjects.Add-Parameter korrigiert, um die richtige Überladung zu verwenden
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

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


