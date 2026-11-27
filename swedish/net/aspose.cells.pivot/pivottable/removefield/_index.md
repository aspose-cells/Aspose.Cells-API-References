---
title: "PivotTable.RemoveField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Tar bort ett fält från ett specifikt fältområde"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Tar bort ett fält från specifikt fältområde

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | PivotFieldType | Fältens områdestyp. |
| fieldName | String | Namnet i basfälten. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Ta bort fältet "c" från Data-området
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // Beräkna pivottabellsdata
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Tar bort ett fält från ett specifikt pivotområde.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | PivotFieldType | Fältens områdestyp. |
| baseFieldIndex | Int32 | Fältindexet i basfälten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Ta bort radfältet (index 0) från pivottabellen
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Ta bort fält från specifikt fältområde

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | PivotFieldType | fältområdestypen. |
| pivotField | PivotField | fältet i basfälten. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Ta bort ett kolumnfält från pivottabellen
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // Ta bort ett datafält från pivottabellen
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // Spara arbetsboken
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


