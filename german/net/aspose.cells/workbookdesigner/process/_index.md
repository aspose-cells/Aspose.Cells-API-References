---
title: "WorkbookDesigner.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Methode. Verarbeitet die Smartmarker und füllt die Werte der Datenquelle."
type: docs
url: /de/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | Range | Der zu verarbeitende Bereich |
| isPreserved | Boolean | True, wenn der nicht erkannte Smartmarker erhalten bleibt. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Range-Smartmarker. Diese Eigenschaft wird 12 Monate nach Juli 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            
            // Beispieldaten in Zellen erstellen
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // WorkbookDesigner erstellen
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // JSON-Datenquelle erstellen
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // Bestimmten Bereich mit Smartmarkern verarbeiten
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // Den Bereich verarbeiten (true = nur diesen Bereich verarbeiten)
            designer.Process(range, true);
            
            // Ergebnis speichern
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle.

```csharp
public void Process()
```

### Beispiele

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // Ein Arbeitsbuch aus einer Vorlagendatei erstellen
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Datenquelle vorbereiten
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // Setze Datenquelle und verarbeite
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle.

```csharp
public void Process(bool isPreserved)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isPreserved | Boolean | True, wenn der nicht erkannte Smartmarker erhalten bleibt. |

### Beispiele

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // Arbeitsbuch initialisieren und Vorlage laden
            Workbook workbook = new Workbook("example.xlsx");
            
            // Beispieldaten direkt erstellen, anstatt sie aus JSON zu laden
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // Richte Smartmarker ein
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // Datenquellen vorbereiten
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // WorkbookDesigner verarbeiten
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // Mit booleschem Parameter verarbeiten
            designer.Process(true);
            
            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }

    // Beispieldatenklassen
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Verarbeitet die Smart‑Marker und füllt die Werte der Datenquelle.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Arbeitsblatt-Index. |
| isPreserved | Boolean | True, wenn der nicht erkannte Smartmarker erhalten bleibt. |

### Hinweise

Diese Methode funktioniert auf Arbeitsblattebene.

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Ein Arbeitsbuch aus einer Quelldatei erstellen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Daten vom Arbeitsblatt in die DataTable exportieren
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // WorkbookDesigner erstellen und Datenquelle festlegen
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // Den Designer mit Parametern (Int32, Boolean) verarbeiten
            designer.Process(0, true);

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


