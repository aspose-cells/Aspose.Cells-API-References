---
title: "WorksheetCollection.AddCopy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem vorhandenen Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt.

```csharp
public int AddCopy(string sheetName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | String | Name des Quellarbeitsblatts. |

### Rückgabewert

[`Worksheet`](../../worksheet/) object index.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [CellsException](../../cellsexception/) | Gibt einen ungültigen Arbeitsblattnamen an. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein Arbeitsblatt mit dem Namen "Original" zum Arbeitsbuch hinzu
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // Fügen Sie einige Daten zum ursprünglichen Arbeitsblatt hinzu
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // Erstelle eine Kopie des "Original" Arbeitsblatts
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // Ändere das kopierte Blatt, um zu zeigen, dass es eine separate Kopie ist
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt.

```csharp
public int AddCopy(int sheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Index des Quellarbeitsblatts. |

### Rückgabewert

[`Worksheet`](../../worksheet/) object index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // Füge eine Kopie des ersten Arbeitsblatts hinzu
            workbook.Worksheets.AddCopy(0);
            
            // Überprüfe, ob die Kopie erstellt wurde
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Kopiert eine Gruppe von Arbeitsblättern.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Worksheet[] | Die Quellarbeitsblätter. |
| destSheetNames | String[] | Die Namen der kopierten Blätter. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge einige Beispielarbeitsblätter hinzu
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Fülle einige Daten in die Arbeitsblätter ein
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Bereite das Quellarbeitsblätter-Array vor
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // Bereite das Zielblattnamen-Array vor
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // Rufe die AddCopy-Methode mit den Parametern (Worksheet[], String[]) auf
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Überprüfe, ob die Kopien erstellt wurden
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


