---
title: "PivotField.HideItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Legt fest, ob das bestimmte PivotItem in einem Datenfeld ausgeblendet ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Legt fest, ob das spezifische PivotItem in einem Datenfeld ausgeblendet ist.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(int index, bool isHidden)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des PivotItem im PivotField. |
| isHidden | Boolean | Ob das spezifische PivotItem ausgeblendet ist |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[int].IsHidden. Diese Methode wird 12 Monate später, seit August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit einer Beispiel‑PivotTable
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten für PivotTable
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("PO-23-05");
            sheet.Cells["A3"].PutValue("PO-23-06");
            sheet.Cells["A4"].PutValue("PO-23-05");
            sheet.Cells["A5"].PutValue("PO-23-07");
            
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(1500);
            sheet.Cells["B5"].PutValue(3000);

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Ausblenden von Elementen, die nicht "PO-23-05" sind
            for (int i = 0; i < pivotField.ItemCount; i++)
            {
                pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
            }
            
            // Pivot-Tabelle berechnen
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldHideItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Legt fest, ob das spezifische PivotItem in einem Datenfeld ausgeblendet ist.

```csharp
[Obsolete("Use PivotField.PivotItems[string].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(string itemValue, bool isHidden)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| itemValue | String | Der Name des pivotItem im pivotField. |
| isHidden | Boolean | Ob das bestimmte PivotItem ausgeblendet ist |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotField.PivotItems[string].IsHidden. Diese Methode wird 12 Monate später, seit August 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodHideItemWithStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Rufen Sie die HideItem-Methode mit den Parametern (String, Boolean) auf
                pivotField.HideItem("Apple", true);

                Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
                Console.WriteLine("Apple items are now hidden in the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HideItem method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


