---
title: "AutoFilter.Custom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Filtrerar en lista med ett anpassat kriterium"
type: docs
url: /sv/net/aspose.cells/autofilter/custom/
---
## Custom(int, FilterOperatorType, object) {#custom}

Filtrerar en lista med ett anpassat kriterium.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| operatorType1 | FilterOperatorType | Filteroperatorens typ |
| criteria1 | Object | Det anpassade kriteriet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kolumn A (10 rader + rubrik)
            worksheet.Cells["A1"].PutValue("Numbers");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i); // A2-A11: 1-10
            }

            // Ange autofilterintervall (A1:A11)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Tillämpa anpassat filter: Nummer > 5
                worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterThan, 5);
                
                // Uppdatera filter för att tillämpa ändringar
                worksheet.AutoFilter.Refresh();
                
                Console.WriteLine("Custom filter applied: Column 0 values > 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }
            
            // Spara den filtrerade arbetsboken
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Custom(int, FilterOperatorType, object, bool, FilterOperatorType, object) {#custom_1}

Filtrerar en lista med anpassade kriterier.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1, bool isAnd, 
    FilterOperatorType operatorType2, object criteria2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| operatorType1 | FilterOperatorType | Filteroperatorens typ |
| criteria1 | Object | Det anpassade kriteriet |
| isAnd | Boolean |  |
| operatorType2 | FilterOperatorType | Filteroperatorens typ |
| criteria2 | Object | Det anpassade kriteriet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata
            worksheet.Cells["A1"].PutValue("Product ID");
            worksheet.Cells["A2"].PutValue(85);
            worksheet.Cells["A3"].PutValue(42);
            worksheet.Cells["A4"].PutValue(65);
            worksheet.Cells["A5"].PutValue(95);
            worksheet.Cells["A6"].PutValue(30);
            worksheet.Cells["A7"].PutValue(75);

            // Ange autofilterintervall (A1:A7)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 0); // Start row: 0 (A1), strartt column: 0 (A), end Column: 0 (A)

            try
            {
                // Tillämpa anpassat filter: Större än eller lika med 50 AND Mindre än eller lika med 100
                autoFilter.Custom(
                    0, // Field index (column A)
                    FilterOperatorType.GreaterOrEqual,
                    50, // First criteria
                    true, // AND combination
                    FilterOperatorType.LessOrEqual,
                    100 // Second criteria
                );

                Console.WriteLine("Custom filter applied successfully with parameters: " +
                    "(Int32, FilterOperatorType, Object, Boolean, FilterOperatorType, Object)");

                // Uppdatera filter och spara resultat
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }

            // Spara den filtrerade arbetsboken
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


