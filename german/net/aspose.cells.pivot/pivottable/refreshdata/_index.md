---
title: "PivotTable.RefreshData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Aktualisiert Daten aus seiner Datenquelle in den Pivot‑Cache."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Aktualisiert Daten aus seiner Datenquelle in den Pivot‑Cache.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### Hinweise

Wir sammeln Daten aus der Datenquelle in einen Pivot-Cache und berechnen dann die Daten im Cache in die Zellen. Und es ist besser, wenn Sie einfach [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) aufrufen, um alle Pivot-Tabellen in der Datei zu aktualisieren und zu berechnen, anstatt sie einzeln zu aktualisieren. HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die [`Refresh`](../../pivotcache/refresh/)‑Methode und entfernen Sie die nachfolgende [`CalculateData`](../calculatedata/), da diese Pivot‑Tabelle beim Aktualisieren des [`PivotCache`](../pivotcache/) berechnet wird. Diese Methode wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilen- und Datenfelder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Pivot-Tabellendaten aktualisieren und berechnen
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Aktualisiert die Daten und Einstellungen der Pivot‑Tabelle aus ihrer Datenquelle mit Optionen.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Option | PivotTableRefreshOption | Die Optionen zum Aktualisieren der Datenquelle der PivotTable. |

### Hinweise

Wir sammeln Daten aus der Datenquelle in einen Pivot-Cache und berechnen dann die Daten im Cache in die Zellen. Und es ist besser, wenn Sie einfach [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) aufrufen, um alle Pivot-Tabellen in der Datei zu aktualisieren und zu berechnen, anstatt sie einzeln zu aktualisieren. HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die [`Refresh`](../../pivotcache/refresh/)‑Methode und entfernen Sie die nachfolgende [`CalculateData`](../calculatedata/), da diese Pivot‑Tabelle beim Aktualisieren des [`PivotCache`](../pivotcache/) berechnet wird. Diese Methode wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greifen Sie auf das Arbeitsblatt zu, das die Pivot‑Tabelle enthält
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // Ermitteln Sie die erste Pivot‑Tabelle im Arbeitsblatt
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Aktualisierungsoptionen konfigurieren
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Aktualisieren Sie die Pivot‑Tabellendaten mit den angegebenen Optionen
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // Speichere die geänderte Arbeitsmappe
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


