---
title: "PivotField.GroupBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gruppiert das Feld automatisch mit Intervall"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

Gruppiert das Feld automatisch mit Intervall

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Intervall | Double | Der interne Wert der Gruppe. Ein automatischer Wert wird zugewiesen, wenn er Null ist, |
| newField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird. Nur für DateTime-Gruppierung. |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions). Diese Methode wird 6 Monate nach September 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Feld zum Spaltenbereich hinzufügen
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Gruppiere das Feld nach 1 (Intervall) mit automatischem Bereich
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

Feld automatisch mit intern gruppieren

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Gruppen | PivotGroupByType[] | Gruppentypen |
| Intervall | Double | Der interne Wert der Gruppe. Ein automatischer Wert wird zugewiesen, wenn er null ist. Funktioniert nur für die Gruppierung nach Zahlen oder Tagen. |
| newField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird. |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions). Diese Methode wird 6 Monate nach September 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Siehe auch

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

Datei nach den Datumsgruppentypen gruppieren.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Start | DateTime | Der Startzeitpunkt |
| Ende | DateTime | Der Endzeitpunkt |
| Gruppen | PivotGroupByType[] | Gruppentypen |
| Intervall | Double | Das Intervall |
| firstAsNewField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird. Nur für das erste Gruppenelement. |

### Rückgabewert

False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions). Diese Methode wird 6 Monate nach September 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Datumsangaben zur Pivot-Tabelle hinzufügen
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields[0];

            // Parameter für die GroupBy-Methode vorbereiten
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // GroupBy-Methode mit Datumsparametern aufrufen
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Pivot-Tabelle aktualisieren
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

Datei nach den Datumsgruppentypen gruppieren.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAutoStart | Boolean | Gibt an, ob der Startzeitwert automatisch erkannt werden soll. |
| Start | DateTime | Der Startzeitpunkt |
| isAutoEnd | Boolean | Gibt an, ob der Endzeitwert automatisch erkannt werden soll. |
| Ende | DateTime | Der Endzeitpunkt |
| Gruppen | PivotGroupByType[] | Gruppentypen |
| Intervall | Double | Das Intervall |
| firstAsNewField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird. Nur für das erste Gruppenelement. |

### Rückgabewert

False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions). Diese Methode wird 6 Monate nach September 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Siehe auch

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

Datei nach Zahl gruppieren.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Start | Double | Der Startwert |
| Ende | Double | Der Endwert |
| Intervall | Double | Das Intervall |
| newField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird |

### Rückgabewert

False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions). Diese Methode wird 6 Monate nach September 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen und gruppieren
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

Datei nach Zahl gruppieren.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAutoStart | Boolean | Gibt an, ob der Startwert automatisch erkannt werden soll. |
| Start | Double | Der Startwert |
| isAutoEnd | Boolean | Gibt an, ob der Endwert automatisch erkannt werden soll. |
| Ende | Double | Der Endwert |
| Intervall | Double | Das Intervall |
| newField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird |

### Rückgabewert

False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions). Diese Methode wird 6 Monate nach September 2026 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Benutzerdefinierte Gruppierung des Feldes.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | Die benutzerdefinierten Gruppenelemente. |
| newField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird |

### Rückgabewert

False bedeutet, dass dieses Feld nicht nach Datum/Zeit gruppiert werden kann.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions options) mit der Eigenschaft PivotFieldGroupOptions.DiscreteGroupItems. Diese Methode wird 6 Monate später, ab Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields[0];

            // Benutzerdefinierte Gruppenelemente erstellen
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Rufen Sie die GroupBy-Methode mit benutzerdefinierten Gruppenelementen auf
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Pivot-Tabelle aktualisieren
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

Benutzerdefinierte Gruppierung des Feldes.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | Die benutzerdefinierten Gruppenelemente. |
| newField | Boolean | Gibt an, ob ein neues Feld zur Pivot-Tabelle hinzugefügt wird |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.Group(PivotFieldGroupOptions options) mit der Eigenschaft PivotFieldGroupOptions.DiscreteGroupItems. Diese Methode wird 6 Monate später, ab Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Siehe auch

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


