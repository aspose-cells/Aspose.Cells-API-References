---
title: "AutoFilter.GetCellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Hämtar CellArea där detta AutoFilter gäller"
type: docs
url: /sv/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

Hämtar [`CellArea`](../../cellarea/) där detta AutoFilter gäller.

```csharp
public CellArea GetCellArea()
```

### Returvärde

området som detta filter gäller för

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i exempeldata för AutoFilter-demonstration
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // Applicera AutoFilter på rubriker (radindex 0) som täcker kolumnerna A-C (0-2)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // Hämta CellArea där AutoFilter tillämpas
                CellArea result = autoFilter.GetCellArea();

                // Skriv ut AutoFilter-områdets koordinater
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // Applicera ett enkelt filter för att demonstrera funktionaliteten (valfritt)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // Spara arbetsboken med tillämpat AutoFilter
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

Hämtar [`CellArea`](../../cellarea/) där det specificerade AutoFilter gäller.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| refreshAppliedRange | Boolean | Om det tillämpade området ska uppdateras. För det tillämpade området för autofilter kan den sista raden ändras när celldata ändras. Om denna flagga är sann, kommer den sista raden i området att beräknas om enligt aktuell celldata. |

### Returvärde

området som detta filter gäller för

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered exempeldata för AutoFilter
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // Ange AutoFilter-område (rad 0 till 3, kolumn 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Anropa GetCellArea med refreshAppliedRange=true
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // Visa det tillämpade området för AutoFilter
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


