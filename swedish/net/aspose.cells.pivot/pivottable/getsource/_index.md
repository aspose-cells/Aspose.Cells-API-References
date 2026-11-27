---
title: "PivotTable.GetSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑metod. Hämta datakällan för denna pivottabell"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Hämta datakällan för denna pivottabell.

```csharp
public string[] GetSource()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Hämta och visa källdataområdet
            string[] sourceData = pivotTable.GetSource();
            Console.WriteLine("Pivot Table Source: " + sourceData[0]);
            
            // Ändra datakällan
            pivotTable.ChangeDataSource(new[] { "A1:B4" });
            
            // Verifiera den ändrade källan
            sourceData = pivotTable.GetSource();
            Console.WriteLine("Updated Pivot Table Source: " + sourceData[0]);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Hämta datakällan för denna pivottabell.

```csharp
public string[] GetSource(bool isOriginal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isOriginal | Boolean | Anger om den ursprungliga eller visade datakällan ska returneras. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Hämta källdata med lokal sökväg (true)
            string[] localSource = pivotTable.GetSource(true);
            Console.WriteLine("Local path source: " + localSource[0]);
            
            // Hämta källdata med fullständig sökväg (false)
            string[] fullSource = pivotTable.GetSource(false);
            Console.WriteLine("Full path source: " + fullSource[0]);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


