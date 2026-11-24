---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Konstruktor. Initialisiert eine neue Instanz der WorkbookDesigner-Klasse"
type: docs
url: /de/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Initialisiert eine neue Instanz der [`WorkbookDesigner`](../)-Klasse.

```csharp
public WorkbookDesigner()
```

### Beispiele

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorDemo
    {
        public static void Run()
        {
            // Eine neue WorkbookDesigner-Instanz mit dem Konstruktor erstellen
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Beispieldatenquelle erstellen
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // Eine neue Arbeitsmappe erstellen und sie als Arbeitsmappe des Designers festlegen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Marker im Arbeitsblatt festlegen
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // Die Arbeitsmappe dem Designer zuweisen
            designer.Workbook = workbook;

            // Setze Datenquelle und verarbeite
            designer.SetDataSource("Level", levels);
            designer.Process();

            // Ergebnis speichern
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    public class Level
    {
        public string Name { get; set; }
        public string Value { get; set; }

        public Level(string name, string value)
        {
            Name = name;
            Value = value;
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Initialisiert eine neue Instanz der [`WorkbookDesigner`](../)-Klasse.

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Arbeitsmappe | Arbeitsmappe | Die Vorlagen-Arbeitsmappe-Datei. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten in Zellen einfügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // JSON-Datenquelle erstellen
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // WorkbookDesigner mit der Arbeitsmappe initialisieren
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // JSON-Datenquelle festlegen
            designer.SetJsonDataSource("ds", jsonData);
            
            // Verarbeite den Designer
            designer.Process();
            
            // Gib das Ergebnis aus
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### Siehe auch

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


