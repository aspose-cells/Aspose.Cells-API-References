---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlTableLoadOptionCollection-Methode. Fügt ein HtmlTableLoadOption zu dieser Sammlung hinzu"
type: docs
url: /de/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Fügt ein HtmlTableLoadOption zu dieser Sammlung hinzu.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | HtmlTableLoadOption | ein HtmlTableLoadOption |

### Rückgabewert

der Index des hinzugefügten Elements

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode AddTableLoadOption(). Diese Methode wird 6 Monate später, seit Dezember 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Tabellennladeoptionen hinzufügen
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Arbeitsmappe mit Optionen laden
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Ausgabe speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Füge ein HtmlTableLoadOption zur Liste hinzu.

```csharp
public int Add(int tableIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableIndex | Int32 | Tabellenindex |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Greife auf die HtmlTableLoadOptionCollection-Instanz zu
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Füge eine neue HtmlTableLoadOption per Tabellenindex hinzu
            int index = tableLoadOptions.Add(0);

            // Zugriff auf das hinzugefügte HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // Erstelle eine Arbeitsmappe und lade HTML mit Optionen
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Füge ein HtmlTableLoadOption zur Liste hinzu.

```csharp
public int Add(string tableId)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableId | String | Tabellen-ID |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Greife auf die HtmlTableLoadOptionCollection-Instanz zu
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Füge eine neue HtmlTableLoadOption per Tabellen-ID hinzu
            int index = tableLoadOptions.Add("mainTable");

            // Zugriff auf das hinzugefügte HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // Arbeitsmappe erstellen und HTML mit Optionen laden
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Füge ein HtmlTableLoadOption zur Liste hinzu.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableIndex | Int32 | Tabellenindex |
| targetSheetIndex | Int32 | Der Zielindex des Arbeitsblatts in Excel |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Tabellen nach Index mit Zielarbeitsblatt-Index hinzufügen
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // HTML-Datei mit den angegebenen Optionen laden
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Füge ein HtmlTableLoadOption zur Liste hinzu.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableId | String | Tabellen-ID |
| targetSheetIndex | Int32 | Der Zielindex des Arbeitsblatts in Excel |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Greife auf die HtmlTableLoadOptionCollection-Instanz zu
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Füge eine neue HtmlTableLoadOption per Tabellen-ID und Zielblattindex hinzu
            int index = tableLoadOptions.Add("tableId", 1);

            // Erstelle eine Arbeitsmappe und lade HTML mit Optionen
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Füge ein HtmlTableLoadOption zur Liste hinzu.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableIndex | Int32 | Tabellenindex |
| targetSheetIndex | Int32 | Der Zielindex des Arbeitsblatts in Excel |
| originalSheetIndex | Int32 | Der ursprüngliche Index des Arbeitsblatts im HTML |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Auf die HtmlTableLoadOptionCollection zugreifen
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Füge eine Tabelle mit Index 1, Zielblatt-Index 1 und Originalblatt-Index 0 hinzu
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // Erstelle eine Arbeitsmappe und lade HTML mit Optionen
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Füge ein HtmlTableLoadOption zur Liste hinzu.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableId | String | Tabellen-ID |
| targetSheetIndex | Int32 | Der Zielindex des Arbeitsblatts in Excel |
| originalSheetIndex | Int32 | Der ursprüngliche Index des Arbeitsblatts im HTML |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Demonstriere die Add-Methode mit den Parametern (String, Int32, Int32)
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // Lade HTML-Datei (ersetze durch tatsächlichen Dateipfad)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


