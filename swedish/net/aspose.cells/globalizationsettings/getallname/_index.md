---
title: "GlobalizationSettings.GetAllName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar namnet på All-etiketten i PivotTable."
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getallname/
---
## GlobalizationSettings.GetAllName method

Hämtar namnet på "(All)"-etiketten i PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfAll() method instead.")]
public virtual string GetAllName()
```

### Returvärde

Namnet på "(All)"-etiketten

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället metoden GlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare sedan december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetAllNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Kom åt instansen för de anpassade inställningarna
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            try
            {
                // Anropa GetAllName-metoden och visa resultatet
                string allName = settings.GetAllName();
                Console.WriteLine($"Custom (All) label: {allName}");

                // Skapa en exempel-pivottabell för att demonstrera lokalanpassningseffekten
                Worksheet worksheet = workbook.Worksheets[0];
                CreateSampleData(worksheet);
                CreatePivotTable(worksheet);

                Console.WriteLine("Demo executed successfully. Check output file's pivot table labels.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("MethodGetAllNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Cars";
            worksheet.Cells["A4"].Value = "Bikes";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["B4"].Value = 1500;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Skapa pivottabell med hjälp av exempeldata
            int pivotIndex = worksheet.PivotTables.Add(
                "PivotTable",
                "A1:B4",
                "E3"
            );
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Konfigurera pivottabellens struktur
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[0]); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[1]); // Sales

            // Uppdatera tabellen för att tillämpa lokalanpassningsinställningarna
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetAllName()
        {
            // Anpassad implementation returnerar den lokalanpassade "All"-etiketten
            return "[Custom All Selection]";
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


