---
title: "PivotTable.GetFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable metod. Hämtar den specifika pivottfältlistan efter regionen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/getfields/
---
## PivotTable.GetFields method

Hämtar den specifika listan med pivotfält efter regionen.

```csharp
public PivotFieldCollection GetFields(PivotFieldType fieldType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | PivotFieldType | regionstypen. |

### Returvärde

den specifika pivottfältsamlingen

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodGetFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Anropa GetFields metod med PivotFieldType.Row parameter
                PivotFieldCollection rowFields = pivotTable.GetFields(PivotFieldType.Row);
                
                Console.WriteLine($"Number of row fields: {rowFields.Count}");
                foreach (PivotField field in rowFields)
                {
                    Console.WriteLine($"Row field name: {field.Name}");
                }

                // Anropa GetFields metod med PivotFieldType.Data parameter
                PivotFieldCollection dataFields = pivotTable.GetFields(PivotFieldType.Data);
                
                Console.WriteLine($"Number of data fields: {dataFields.Count}");
                foreach (PivotField field in dataFields)
                {
                    Console.WriteLine($"Data field name: {field.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFields method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("PivotTableGetFieldsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


