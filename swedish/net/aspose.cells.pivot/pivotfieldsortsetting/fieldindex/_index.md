---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldSortSetting-egenskap. Representerar indexet för fältet som sorteras efter. 1 betyder att sortera PivotField efter etiketter, andra betyder sortering efter datafältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

Representerar indexet för fältet som sorteras efter. -1 betyder att sortera PivotField efter etiketter, andra betyder sortering efter datafältet.

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället PivotFieldSortSetting.SortBy-egenskap. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Hämta pivottfältets sorteringsinställning
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // Visa aktuellt FieldIndex-värde
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // Obs: FieldIndex är skrivskyddad och PivotFieldSortSetting kan inte instansieras direkt
            // eftersom den saknar offentlig konstruktor. Vi kan bara arbeta med den befintliga instansen
            // hämtad från pivottfältets SortSetting-egenskap.

            // Uppdatera pivottabellen för att tillämpa ändringarna
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara resultatet
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


