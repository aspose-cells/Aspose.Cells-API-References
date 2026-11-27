---
title: "PivotTable.AddFieldToArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Lägger till fältet i det specifika området"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/addfieldtoarea/
---
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}

Lägger till fältet i det specifika området.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | PivotFieldType | Fältens områdestyp. |
| fieldName | String | Namnet i basfälten. |

### Returvärde

Fältpositionen i de specifika fälten.Om det inte finns något fält med det namnet, returnera -1.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "P1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "P2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            cells["A4"].Value = "P3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 2000;
            cells["A5"].Value = "P1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 1200;

            // Lägg till en pivottabell
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // Lägg till fält i olika områden med AddFieldToArea med fältnamn som strängar
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Column, "Region");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera och beräkna pivottabell
            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableDemo_out.xlsx");
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

## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}

Lägger till fältet i det specifika området.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | PivotFieldType | Fältens områdestyp. |
| baseFieldIndex | Int32 | Indexet i basfälten. |

### Returvärde

Fältpositionen i de specifika fälten.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Product " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue("Region " + (i % 2 + 1));
                worksheet.Cells["C" + i].PutValue(i * 100);
            }

            // Lägg till en pivottabell
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Lägg till fält i områden med AddFieldToArea(PivotFieldType, Int32)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data field

            // Spara arbetsboken
            workbook.Save("PivotTableDemo_out.xlsx");
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

## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}

Lägger till fältet i det specifika området.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | PivotFieldType | fältområdestypen. |
| pivotField | PivotField | fältet i basfälten. |

### Returvärde

fältpositionen i de specifika fälten.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad med källdata
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "Source Data";
            
            // Lägg till exempeldata
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Region");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Product A");
            sourceSheet.Cells["B2"].PutValue("North");
            sourceSheet.Cells["C2"].PutValue(1000);
            
            sourceSheet.Cells["A3"].PutValue("Product B");
            sourceSheet.Cells["B3"].PutValue("South");
            sourceSheet.Cells["C3"].PutValue(2000);
            
            sourceSheet.Cells["A4"].PutValue("Product A");
            sourceSheet.Cells["B4"].PutValue("East");
            sourceSheet.Cells["C4"].PutValue(1500);
            
            sourceSheet.Cells["A5"].PutValue("Product B");
            sourceSheet.Cells["B5"].PutValue("West");
            sourceSheet.Cells["C5"].PutValue(2500);

            // Lägg till en pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            string source = "='Source Data'!A1:C5";
            int index = pivotTables.Add(source, "A1", "PivotTable");
            PivotTable pTable = pivotTables[index];

            // Lägg till fält i områden
            pTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pTable.AddFieldToArea(PivotFieldType.Row, 1); // Region
            
            // Lägg till datafält
            pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pTable.DataFields[0].Function = ConsolidationFunction.Sum;
            pTable.DataFields[0].NumberFormat = "$0.00";

            // Lägg till datafält till kolumnområdet med PivotField-parameter
            if (pTable.DataField != null)
            {
                pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
            }

            // Spara arbetsboken
            workbook.Save("PivotTableDemo.xlsx");
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


