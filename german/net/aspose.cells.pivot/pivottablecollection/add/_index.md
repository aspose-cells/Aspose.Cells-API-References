---
title: "PivotTableCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTableCollection-Methode. Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition im Arbeitsblatt mit Standardoptionen hinzu."
type: docs
url: /de/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string) {#add_2}

Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition im Arbeitsblatt mit Standardoptionen hinzu.

```csharp
public PivotTable Add(string sourceData, string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| cellName | String | Der Name der Zelle in der oberen linken Ecke für das PivotTable-Ziel. |

### Rückgabewert

Die neu erstellte PivotTable-Instanz.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, PivotTableCreateOptions) {#add_3}

Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition im Arbeitsblatt mit Standardoptionen hinzu.

```csharp
public PivotTable Add(string sourceData, string cellName, PivotTableCreateOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| cellName | String | Der Name der Zelle in der oberen linken Ecke für das PivotTable-Ziel. |
| Optionen | PivotTableCreateOptions | Die Optionen zum Erstellen einer PivotTable. |

### Rückgabewert

Die neu erstellte PivotTable-Instanz.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add}

Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition im Arbeitsblatt mit Standardoptionen hinzu.

```csharp
public PivotTable Add(string sourceData, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| row | Int32 | Der nullbasierte Zeilenindex der oberen linken Ecke für das PivotTable-Ziel. |
| column | Int32 | Der nullbasierte Spaltenindex der oberen linken Ecke für das PivotTable-Ziel. |

### Rückgabewert

Die neu erstellte PivotTable-Instanz.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, PivotTableCreateOptions) {#add_1}

Fügt eine neue PivotTable an der angegebenen Zeilen‑ und Spaltenposition im Arbeitsblatt hinzu.

```csharp
public PivotTable Add(string sourceData, int row, int column, PivotTableCreateOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| row | Int32 | Der nullbasierte Zeilenindex der oberen linken Ecke für das PivotTable-Ziel. |
| column | Int32 | Der nullbasierte Spaltenindex der oberen linken Ecke für das PivotTable-Ziel. |
| Optionen | PivotTableCreateOptions | PivotTable-Erstellungsoptionen. |

### Rückgabewert

Die neu erstellte PivotTable-Instanz.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_9}

Fügt eine neue PivotTable mit dem Legacy-Layout und -Stil von Excel 97-2003 hinzu.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Die Daten für den neuen PivotTable-Cache. |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der Index in dieser PivotTable-Liste.

### Hinweise

HINWEIS: Diese Methode ist veraltet. Sie ist äquivalent zum Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe aus der Quell‑CSV
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "SourceData";
            
            // Fügen Sie Beispieldaten hinzu
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Value");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(10);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(20);
            sourceSheet.Cells["A4"].PutValue("A");
            sourceSheet.Cells["B4"].PutValue(30);

            // PivotTable-Arbeitsblatt erstellen
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Hole den Quelldatenbereich
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
            string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
            
            // Füge eine PivotTable mit den Parametern String, String, String hinzu
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
            
            // PivotTable konfigurieren
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_10}

Fügt eine neue PivotTable mit dem Legacy-Layout und -Stil von Excel 97-2003 hinzu.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, string, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Die Daten für den neuen PivotTable-Cache. |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | Boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits nutzt. Wenn die Eigenschaft true ist, spart sie Speicher. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Hinweise

HINWEIS: Diese Methode ist veraltet. Sie ist äquivalent zum Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Definiere Parameter für die Add-Methode
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // Rufe die Add-Methode mit den Parametern (String, String, String, Boolean) auf
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // PivotTable konfigurieren
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_6}

Fügt eine neue PivotTable mit dem Legacy-Layout und -Stil von Excel 97-2003 hinzu.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Zellbereich der Daten für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der Index in dieser PivotTable-Liste.

### Hinweise

HINWEIS: Diese Methode ist veraltet. Sie ist äquivalent zum Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein Arbeitsblatt für Daten hinzu
            Worksheet dataWorksheet = workbook.Worksheets[0];
            dataWorksheet.Name = "Data";
            
            // Fügen Sie Beispieldaten hinzu
            dataWorksheet.Cells["A1"].PutValue("Category");
            dataWorksheet.Cells["B1"].PutValue("Product");
            dataWorksheet.Cells["C1"].PutValue("Sales");
            
            dataWorksheet.Cells["A2"].PutValue("Electronics");
            dataWorksheet.Cells["B2"].PutValue("Laptop");
            dataWorksheet.Cells["C2"].PutValue(1000);
            
            dataWorksheet.Cells["A3"].PutValue("Electronics");
            dataWorksheet.Cells["B3"].PutValue("Phone");
            dataWorksheet.Cells["C3"].PutValue(800);
            
            dataWorksheet.Cells["A4"].PutValue("Furniture");
            dataWorksheet.Cells["B4"].PutValue("Chair");
            dataWorksheet.Cells["C4"].PutValue(200);
            
            // Füge ein Arbeitsblatt für die PivotTable hinzu
            Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
            
            // Füge eine PivotTable mit der Add-Methode und den Parametern (String, Int32, Int32, String) hinzu
            string pivotDataRange = "Data!A1:C4";
            int row = 0;
            int column = 0;
            string tableName = "SalesPivotTable";
            
            int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
            
            // Zugriff auf die PivotTable
            PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
            
            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Lege die Konsolidierungsfunktion fest
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
            
            // Pivot-Tabellendaten aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_7}

Fügt eine neue PivotTable mit dem Legacy-Layout und -Stil von Excel 97-2003 hinzu.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Zellbereich der Daten für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | Boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits nutzt. Wenn die Eigenschaft true ist, spart sie Speicher. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Hinweise

HINWEIS: Diese Methode ist veraltet. Sie ist äquivalent zum Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // Definiere den Datenbereich
            string sourceData = "A1:C4";
            
            try
            {
                // Rufen Sie die Add-Methode mit den Parametern auf: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // Greifen Sie auf die neu erstellte Pivot-Tabelle zu
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // PivotTable konfigurieren
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_8}

Fügt eine neue PivotTable mit dem Legacy-Layout und -Stil von Excel 97-2003 hinzu.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Zellbereich der Daten für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | Boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits nutzt. Wenn die Eigenschaft true ist, spart sie Speicher. |
| isXlsClassic | Boolean | Gibt an, ob eine klassische Pivot-Tabelle von Excel 97-2003 hinzugefügt wird. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Hinweise

HINWEIS: Diese Methode ist veraltet. Sie ist äquivalent zum Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach Oktober 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // Definieren Sie den Quell-Datenbereich
            string sourceData = "A1:C5";

            try
            {
                // Rufen Sie die Add-Methode mit den Parametern auf (String, Int32, Int32, String, Boolean, Boolean)
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // PivotTable konfigurieren
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_11}

Fügt eine neue PivotTable hinzu.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Zellbereich der Daten für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| Zelle | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | Boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits nutzt. Ist die Eigenschaft true, spart dies Speicher, wenn dieselbe Datenquelle in einem Pivot-Cache zusammengefasst wurde. |
| isXlsClassic | Boolean | Gibt an, ob eine klassische Pivot-Tabelle von Excel 97-2003 hinzugefügt wird. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Hinweise

HINWEIS: Diese Methode ist veraltet. Sie ist äquivalent zum Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach Oktober 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten befüllen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                cells["A" + i].PutValue("Cat" + (i % 3 + 1));
                cells["B" + i].PutValue("Prod" + i);
                cells["C" + i].PutValue(i * 100);
            }

            // PivotTable mit angegebenen Parametern hinzufügen
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
            
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | PivotTable | Die Quell-PivotTable. |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der Index der neu hinzugefügten PivotTable.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Erstellen Sie eine PivotTable aus dem Datenbereich
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // Rufen Sie die Add-Methode mit den Parametern auf (PivotTable, String, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Arbeitsmappe speichern, um den Effekt zu zeigen
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_4}

Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | PivotTable | Die Quell-PivotTable. |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der Index der neu hinzugefügten PivotTable.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Erstellen Sie eine Quell-PivotTable
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Rufen Sie die Add-Methode mit den Parametern auf (PivotTable, Int32, Int32, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Arbeitsmappe speichern, um den Effekt zu zeigen
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_13}

Fügt ein neues PivotTable‑Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String[] | Die mehreren Konsolidierungsbereiche, z. B. {\"Sheet1!A1:C8\",\"Sheet2!A1:B8\"} |
| isAutoPage | Boolean | Gibt an, ob automatisch ein einzelnes Seitenfeld erstellt wird. Ist true, wird der folgende Parameter pageFields ignoriert. |
| pageFields | PivotPageFields | Die Pivot-Seitenfeld-Elemente. |
| destCellName | String | destCellName Der Name des neuen PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der Index der neu hinzugefügten PivotTable.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // Datenbereich definieren
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // Rufen Sie die Add-Methode mit angegebenen Parametern auf
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Greifen Sie auf die neu erstellte Pivot-Tabelle zu
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Konfiguriere PivotTable-Felder
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_12}

Fügt ein neues PivotTable‑Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String[] | Die mehreren Konsolidierungsbereiche, z. B. {\"Sheet1!A1:C8\",\"Sheet2!A1:B8\"} |
| isAutoPage | Boolean | Ob ein einzelnes Seitenfeld automatisch erstellt wird. Wenn true, wird der folgende Parameter pageFields ignoriert |
| pageFields | PivotPageFields | Die Pivot-Seitenfeld-Elemente. |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der Index der neu hinzugefügten PivotTable.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // Definiere Parameter für die Add-Methode
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // Rufen Sie die Add-Methode mit angegebenen Parametern auf
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // PivotTable konfigurieren
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // Daten aktualisieren
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


