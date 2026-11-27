---
title: "PivotField.SortBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField‑metod. Sorterar detta pivottfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

Sorterar detta pivottfält.

```csharp
public void SortBy(SortOrder sortType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | SortOrder | Typen av sortering för detta fält. |

### Se även

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

Sorterar detta pivottfält.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | SortOrder | Typen av sortering för detta fält. |
| fieldSortedBy | Int32 | Indexet för pivottfältet som sorteras efter. -1 betyder sortering efter datalabels för detta fält, andra värden betyder indexet för datafältet som sorteras efter. |

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortBy(SortOrder, int,string)-metoden eller PivotField.IsAutoSort‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Sortera radfältet i fallande ordning med index -1
            rowField.SortBy(SortOrder.Descending, -1);
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

Sorterar detta pivottfält.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | SortOrder | Typen av sortering för detta fält. |
| fieldSortedBy | Int32 | Indexet för pivottfältet som sorteras efter. -1 betyder sortering efter datalabels för detta fält, andra värden betyder indexet för datafältet som sorteras efter. |
| dataType | PivotLineType | Typen av data som sorteras efter. |
| cellName | String | Sortera efter värden i raden eller kolumnen |

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortBy(SortOrder, int,string)-metoden. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Sortera radfältet
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // Beräkna data
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

Sorterar detta pivottfält.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sortType | SortOrder | Typen av sortering för detta fält. |
| fieldSortedBy | Int32 | Indexet för pivottfältet som sorteras efter. -1 betyder sortering efter datalabels för detta fält, andra värden betyder indexet för datafältet som sorteras efter. |
| cellName | String | Sortera efter värden i raden eller kolumnen. Om Null, gruppera efter fältets total, annars gruppera efter värden i den valda kolumnen eller raden. |

### Se även

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


