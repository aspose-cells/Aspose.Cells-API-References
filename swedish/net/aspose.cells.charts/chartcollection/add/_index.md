---
title: "ChartCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartCollection-metod. Lägger till ett diagram i samlingen"
type: docs
url: /sv/net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Lägger till ett diagram i samlingen.

```csharp
public int Add(ChartType type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ChartType | Diagramtyp |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| bottomRow | Int32 | Index för nedre högra rad |
| rightColumn | Int32 | Index för nedre högra kolumnen |

### Returvärde

[`Chart`](../../chart/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 1; i <= 10; i++)
            {
                sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                sheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Lägg till ett diagram med de angivna parametrarna
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Lägger till ett diagram i samlingen.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ChartType | Diagramtyp |
| dataRange | String | Anger diagrammets dataområde |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| rightRow | Int32 | Index för nedre högra rad |
| bottomColumn | Int32 | Index för nedre högra kolumnen |

### Returvärde

[`Chart`](../../chart/) object index.

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället `Add`-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan maj 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Anropa Add-metoden med parametrarna (ChartType, String, Int32, Int32, Int32, Int32)
                int chartIndex = worksheet.Charts.Add(
                    ChartType.Column,          // Chart type
                    "A1:B4",                  // Data range
                    0,                        // Top row position
                    3,                        // Left column position
                    15,                       // Bottom row position
                    8                         // Right column position
                );

                Console.WriteLine("Chart added successfully at index: " + chartIndex);
                
                // Få åtkomst till det nyss skapade diagrammet
                Chart chart = worksheet.Charts[chartIndex];
                chart.Title.Text = "Sample Column Chart";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ChartCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Lägger till ett diagram med förinställd mall.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| data | Byte[] | Data för diagrammallfil (.crtx). |
| dataRange | String | Anger diagrammets dataområde |
| ärVertikal | Boolean | Anger om serien ska plottas från ett område med cellvärden radvis eller kolumnvis. |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| rightRow | Int32 | Index för nedre högra rad |
| bottomColumn | Int32 | Index för nedre högra kolumnen |

### Returvärde

[`Chart`](../../chart/) object index.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i arbetsbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Skapa en byte-array som representerar diagramdata (förenklat exempel)
            byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };

            try
            {
                // Anropa Add-metoden med specifika parametrar
                int chartIndex = worksheet.Charts.Add(
                    chartData,          // Byte[] data
                    "A1:B4",            // String dataRange
                    true,               // Boolean isVertical
                    0,                  // Int32 topRow
                    0,                  // Int32 leftColumn
                    15,                 // Int32 rightRow
                    8                   // Int32 bottomColumn
                );

                Console.WriteLine($"Chart added successfully at index: {chartIndex}");

                // Få åtkomst till det tillagda diagrammet
                Chart chart = worksheet.Charts[chartIndex];
                chart.Type = ChartType.Column;

                // Spara resultatet
                workbook.Save("ChartCollectionMethodAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Lägger till ett diagram i samlingen.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ChartType | Diagramtyp |
| dataRange | String | Anger diagrammets dataområde |
| ärVertikal | Boolean | Anger om serien ska plottas från ett område med cellvärden radvis eller kolumnvis. |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| rightRow | Int32 | Index för nedre högra rad |
| bottomColumn | Int32 | Index för nedre högra kolumnen |

### Returvärde

[`Chart`](../../chart/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);

            // Lägg till diagram med angivna parametrar
            int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


