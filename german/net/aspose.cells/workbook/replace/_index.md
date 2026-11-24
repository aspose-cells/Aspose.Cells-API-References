---
title: "Workbook.Replace"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Ersetzt den Wert einer Zelle durch einen neuen String"
type: docs
url: /de/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Ersetzt den Wert einer Zelle durch einen neuen String.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValue | String | String-Wert zum Ersetzen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // Ersetze alle Vorkommen von "Apple" durch "Mango"
            workbook.Replace("Apple", "Mango");
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Ersetzt den Wert einer Zelle durch einen neuen Integer.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValue | Int32 | Ganzzahlwert zum Ersetzen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // Ersetze alle Vorkommen von "OriginalValue" durch die Ganzzahl 100
            workbook.Replace("OriginalValue", 100);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Ersetzt den Wert einer Zelle durch einen neuen Double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValue | Double | Double-Wert zum Ersetzen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Beispieldaten in Zellen ein
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Ersetze Text durch Double-Wert
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Ersetzt den Wert einer Zelle durch ein neues String-Array.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValues | String[] | String-Array zum Ersetzen |
| isVertical | Boolean | True - Vertikal, False - Horizontal |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einigen Zellen Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Definiere neue Werte zum Ersetzen
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // Ersetze alle Vorkommen von "AnOldValue" durch die neuen Werte
            workbook.Replace("AnOldValue", newValues, true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Ersetzt die Werte der Zellen durch ein Integer-Array.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValues | Int32[] | Ganzzahl-Array zum Ersetzen |
| isVertical | Boolean | True - Vertikal, False - Horizontal |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einigen Zellen Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // Ersetzungswerte definieren
            int[] newValues = new int[] { 1, 2, 3 };
            
            // Ersetze "OldValue" durch das Array von Ganzzahlen
            workbook.Replace("OldValue", newValues, true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Ersetzt die Werte der Zellen durch ein Double-Array.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValues | Double[] | Double-Array zum Ersetzen |
| isVertical | Boolean | True - Vertikal, False - Horizontal |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Ersetzungswerte definieren
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // Ersetze alle Vorkommen von "AnOldValue" durch die neuen Werte
            workbook.Replace("AnOldValue", newValues, true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Ersetzt die Werte der Zellen durch Daten aus einer DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| insertTable | DataTable | DataTable zum Ersetzen |

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDataTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle ein Beispiel-DataTable
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // Füge Beispieldaten zum DataTable hinzu
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // Füge etwas Text zum Arbeitsblatt hinzu, der ersetzt wird
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // Ersetze den Text durch DataTable
            workbook.Replace("CustomerData", dataTable);
            
            // Speichere die Arbeitsmappe
            workbook.Save("Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Ersetzt die Werte der Zellen durch neue Daten.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| boolValue | Boolean | Der boolesche Wert, der ersetzt werden soll. |
| newValue | Object | Neuer Wert. Kann ein String, Integer, Double oder DateTime-Wert sein. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fülle einige Zellen mit booleschen Werten
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Rufe die Replace-Methode auf, um alle 'true'-Werte durch \"REPLACED\" zu ersetzen
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Ergebnisse anzeigen
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Ersetzt die Werte der Zellen durch neue Daten.

```csharp
public int Replace(int intValue, object newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| intValue | Int32 | Der Integer-Wert, der ersetzt werden soll. |
| newValue | Object | Neuer Wert. Kann ein String, Integer, Double oder DateTime-Wert sein. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fülle einige Zellen mit Integer-Werten, die ersetzt werden sollen
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Rufe die Replace-Methode mit den Parametern (Int32, Object) auf
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Zeige den Inhalt des Arbeitsblatts nach dem Ersetzen an
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Ersetzt den Wert einer Zelle durch einen neuen String.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValue | String | String-Wert zum Ersetzen |
| Optionen | ReplaceOptions | Die Ersetzungsoptionen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false
            };

            int replacedCount = workbook.Replace("Hello", "Hi", options);

            Console.WriteLine($"Replacements made: {replacedCount}");
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


