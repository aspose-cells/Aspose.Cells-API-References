---
title: "PivotField.ShowValuesAs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Zeigt Werte des Datenfelds in einem anderen Anzeigeformat an, wenn die ShowDataAs‑Berechnung verwendet wird."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

Zeigt Werte des Datenfelds in einem anderen Anzeigeformat an, wenn die ShowDataAs‑Berechnung verwendet wird.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | Der Typ des Datenanzeigeformats. |
| baseField | Int32 | Der Index des Feldes, auf dem die ShowDataAs‑Berechnung basiert. |
| baseItemPositionType | PivotItemPositionType | Der Positionstyp des Basis‑Elements. |
| baseItem | Int32 | Der Index des Basiselements, auf dem die ShowDataAs‑Berechnung basiert. Funktioniert nur, wenn baseItemPositionType benutzerdefiniert ist. |

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Diese Methode wird 12 Monate später, seit November 2026, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Fügen Sie Beispieldaten hinzu
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

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Spaltenfeld hinzufügen
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Datenfeld hinzufügen und ShowValuesAs konfigurieren
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Daten berechnen und speichern
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Legt die Berechnung "Werte anzeigen als" für dieses Pivotfeld fest.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Typ der "Show Values As"‑Berechnung. |
| baseField | Int32 | Index des Basisfeldes, das für die Berechnung verwendet wird. |
| baseItem | Int32 | Index des Basiselements für die Berechnung. Verwenden Sie [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) für das vorherige Element, [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) für das nächste Element; nicht‑negative Werte bezeichnen den ordinalen Index eines bestimmten Pivot‑Elements. |

### Hinweise

Nur für Datenfeld.

### Siehe auch

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Konfiguriert die Berechnung "Werte anzeigen als" für dieses Datenfeld.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Der Berechnungstyp für Show Values As. |
| baseField | String | Der Name des Basisfeldes, das in der Berechnung verwendet wird. |
| baseItem | String | Beschriftung eines regulären Pivot‑Elements. Akzeptiert außerdem reservierte Schlüsselwörter: `(previous)` für das vorherige Element, `(next)` für das nächste Element. Geben Sie `null` an, wenn der ausgewählte Berechnungstyp kein Basiselement benötigt. |

### Siehe auch

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


