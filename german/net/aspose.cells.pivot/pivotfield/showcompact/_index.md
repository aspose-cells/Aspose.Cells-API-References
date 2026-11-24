---
title: "PivotField.ShowCompact"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob die Bezeichnungen des nächsten Feldes in derselben Spalte in der Pivot-Tabellenansicht angezeigt werden. Nur für Zeilenfelder"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Gibt an, ob die Bezeichnungen des nächsten Feldes in derselben Spalte in der Pivot-Tabellenansicht angezeigt werden. Nur für Zeilenfelder.

```csharp
[Obsolete("Use PivotField.ShowInCompactForm instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowCompact { get; set; }
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.ShowInCompactForm. Diese Methode wird 12 Monate später, seit November 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowCompactDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Orange");
            worksheet.Cells["A6"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(250);
            worksheet.Cells["B6"].PutValue(300);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A7", "A1:B6", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Fügen Sie ein Zeilenfeld hinzu und konfigurieren Sie ShowCompact
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.ShowInOutlineForm = true;
            rowField.ShowCompact = true;
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot‑Tabelle berechnen und aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldShowCompactDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


