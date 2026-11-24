---
title: "GlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings‑Methode. Gibt den Typnamen von Tabellenzeilen zurück, die aus der Tabellenkopfzeile bestehen. Standard ist Headers, sodass in Formeln Headers die Tabellenkopfzeile darstellt."
type: docs
url: /de/net/aspose.cells/globalizationsettings/gettablerowtypeofheaders/
---
## GlobalizationSettings.GetTableRowTypeOfHeaders method

Gibt den Typnamen von Tabellenzeilen zurück, die die Tabellenüberschrift enthalten. Standard ist "Headers", sodass in der Formel "#Headers" die Tabellenüberschrift darstellt.

```csharp
public virtual string GetTableRowTypeOfHeaders()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTableRowTypeOfHeaders()
            {
                return "MyHeaders";
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 1.8;

            // Behebung der ListObject-Erstellung durch Behandlung des Rückgabewerts von Add()
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            // Verwende die DisplayName‑Eigenschaft anstelle von Name
            table.DisplayName = "FruitTable";

            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                worksheet.Cells["A5"].Formula = "=COUNTA(FruitTable[#MyHeaders])";
                workbook.CalculateFormula();
                Console.WriteLine("Method executed successfully. Header count: " + worksheet.Cells["A5"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


