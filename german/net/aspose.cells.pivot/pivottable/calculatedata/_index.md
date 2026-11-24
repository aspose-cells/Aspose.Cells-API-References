---
title: "PivotTable.CalculateData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Berechnet die Daten der Pivot‑Tabelle in Zellen."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

Berechnet die Daten der PivotTable in Zellen.

```csharp
public void CalculateData()
```

### Hinweise

Diese Methode berechnet Daten nur mit den im [`PivotCache`](../pivotcache/) zwischengespeicherten Daten. Wenn Sie mit der neuesten Datenquelle berechnen möchten, verwenden Sie bitte die [`Refresh`](../../pivotcache/refresh/)‑Methode. Wenn nur die Einstellung der Pivot‑Tabelle geändert wurde, ist `CalculateData` ausreichend.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Pivot‑Tabelle erstellen – behoben durch Sicherstellung korrekter Parameter.
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Felder zur Pivot hinzufügen.
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Datumsfilter anwenden.
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Pivot‑Daten berechnen.
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

Berechnet die PivotTable mit Optionen.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Option | PivotTableCalculateOption | Die Optionen zur Berechnung der Pivot‑Tabelle. |

### Rückgabewert

Gibt alle Pivot‑Tabellen zurück, die berechnet wurden. Wenn [`RefreshData`](../../pivottablecalculateoption/refreshdata/) true ist, werden alle Pivot‑Tabellen, die auf demselben Pivot‑Cache basieren, zusammen berechnet.

### Hinweise

Wenn [`RefreshData`](../../pivottablecalculateoption/refreshdata/) true ist, wird diese Methode den Pivot‑Cache aus der Datenquelle aktualisieren und anschließend alle Pivot‑Tabellen basierend auf demselben Pivot‑Cache berechnen. Andernfalls wird nur mit den im Pivot‑Cache zwischengespeicherten Daten berechnet.

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Setzen Sie Berechnungsoptionen
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Berechne mit Optionen
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


