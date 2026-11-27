---
title: "PivotTableCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableCollection-egenskap. Hämtar PivotTable-rapporten efter index"
type: docs
url: /sv/net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Hämtar PivotTable-rapporten efter index.

```csharp
public PivotTable this[int index] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en arbetsbok från källfil
            Workbook workbook = new Workbook("example.xlsx");
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till pivottabellsamling
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Åtkomst till första pivottabellen med Item-egenskapen (indexerare)
            PivotTable pivotTable = pivotTables[0];
            
            // Beräkna pivottabellsdata
            pivotTable.CalculateData();
            
            // Spara den modifierade arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (2 of 3)

Hämtar PivotTable-rapporten efter pivottabellens namn.

```csharp
public PivotTable this[string name] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(3000);

            // Lägg till en pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Konfigurera pivottabell med Item property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Få åtkomst till pivottabell med Item property
            PivotTable tableFromCollection = sheet.PivotTables["PivotTable1"];
            Console.WriteLine("Pivot table data source: " + string.Join(", ", tableFromCollection.DataSource));

            // Ändra data och uppdatera
            sheet.Cells["B2"].PutValue(1500);
            tableFromCollection.RefreshData();
            Console.WriteLine("Updated pivot table values");

            // Spara arbetsboken
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (3 of 3)

Hämtar [`PivotTable`](../../pivottable/) som finns i cellen.

```csharp
public PivotTable this[int row, int column] { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 3000;

            try
            {
                // Lägg till en pivottabell i kalkylbladet
                int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");

                // Åtkomst till PivotTableCollection
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Visa åtkomst till en pivottabell med Item property (indexer)
                PivotTable pivotTable = pivotTables[index];
                Console.WriteLine($"Accessed pivot table at index {index} with name: {pivotTable.Name}");

                // Visa åtkomst efter namn med Item property
                PivotTable pivotTableByName = pivotTables["PivotTable1"];
                Console.WriteLine($"Accessed pivot table by name: {pivotTableByName.Name}");

                // Konfigurera pivottabellen
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Uppdatera och beräkna data
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Spara arbetsboken
                workbook.Save("PivotTableItemDemo.xlsx");
                Console.WriteLine("Pivot table demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


