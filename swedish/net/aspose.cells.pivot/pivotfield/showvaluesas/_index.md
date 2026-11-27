---
title: "PivotField.ShowValuesAs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Visar värden för datafältet i olika visningsformat när ShowDataAs-beräkningen används"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

Visar värden för datafältet i olika visningsformat när ShowDataAs-beräkningen används.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | Datavisningsformatstypen. |
| baseField | Int32 | Indexet till fältet som ShowDataAs‑beräkningen baseras på. |
| baseItemPositionType | PivotItemPositionType | Positionstypen för bas‑objektet. |
| baseItem | Int32 | Indexet till basobjektet som ShowDataAs‑beräkningen baseras på. Fungerar endast när baseItemPositionType är anpassad. |

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd i stället PivotField.ShowValuesAs(PivotShowValuesAsType,int,int)-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Lägg till radfält
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Lägg till kolumnfält
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Lägg till datafält och konfigurera ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Beräkna data och spara
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Anger beräkningen "Show Values As" för detta pivottfält.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Typ av "Show Values As"‑beräkning. |
| baseField | Int32 | Index för basfältet som används i beräkningen. |
| baseItem | Int32 | Index för basobjektet i beräkningen. Använd [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) för föregående objekt, [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) för nästa objekt; icke‑negativa värden betecknar det ordningsmässiga indexet för ett specifikt pivot‑objekt. |

### Anmärkningar

Endast för datafält.

### Se även

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Konfigurerar beräkningen "Show Values As" för detta datafält.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Beräkningstypen för Show Values As. |
| baseField | String | Namnet på basfältet som används i beräkningen. |
| baseItem | String | Rubrik för ett vanligt pivot‑objekt. Accepterar också reserverade nyckelord: `(previous)` för föregående objekt, `(next)` för nästa objekt. Skicka `null` om den valda beräkningstypen inte kräver ett basobjekt. |

### Se även

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


