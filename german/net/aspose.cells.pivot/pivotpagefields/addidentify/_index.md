---
title: "PivotPageFields.AddIdentify"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotPageFields-Methode. Legt fest, welche Elementbezeichnung in jedem Seitenfeld verwendet wird, um den Datenbereich zu identifizieren. pageItemIndex.Length muss gleich PageFieldCount sein, daher bitte zuerst das Seitenfeld hinzufügen."
type: docs
url: /de/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Legt fest, welches Elementlabel in jedem Seitenfeld verwendet wird, um den Datenbereich zu identifizieren. Die pageItemIndex.Length muss gleich PageFieldCount sein, daher fügen Sie bitte zuerst das Seitenfeld hinzu.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeIndex | Int32 | Der Index des Konsolidierungsdatenbereichs. |
| pageItemIndex | Int32[] | Der Seiten-Element-Index in jedem Seitenfeld. pageItemIndex[2] = 1 bedeutet, dass das zweite Element im dritten Feld verwendet wird, um diesen Bereich zu identifizieren. pageItemIndex[1] = -1 bedeutet, dass kein Element im zweiten Feld verwendet wird, um diesen Bereich zu identifizieren, und MS wird automatisch ein "blank" Element im zweiten Feld erstellen, um diesen Bereich zu identifizieren. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Instanziiere PivotPageFields direkt, anstatt über PivotTable zuzugreifen.
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


