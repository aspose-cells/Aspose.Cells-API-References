---
title: "Worksheet.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Kopiert Inhalte und Formate von einem anderen Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Kopiert Inhalte und Formate von einem anderen Arbeitsblatt.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceSheet | Arbeitsblatt | Quellarbeitsblatt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // Erstelle ein Quell‑Arbeitsbuch mit Beispieldaten
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // Erstelle eine Ziel-Arbeitsmappe.
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Kopieren Sie das Quellarbeitsblatt in das Zielarbeitsblatt
            destSheet.Copy(sourceSheet);
            
            // Ergebnis speichern
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Kopiert Inhalte und Formate von einem anderen Arbeitsblatt.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceSheet | Arbeitsblatt | Quellarbeitsblatt. |
| copyOptions | CopyOptions |  |

### Hinweise

Sie können Daten von einem anderen Arbeitsblatt in derselben Datei oder einer anderen Datei kopieren. Diese Methode unterstützt jedoch nicht das Kopieren von Zeichenobjekten, wie Kommentaren, Bildern und Diagrammen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // Erstelle eine Quell-Arbeitsmappe mit Beispieldaten.
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // Kopieroptionen konfigurieren
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // Arbeitsblatt mit Optionen kopieren
            srcSheet.Copy(destSheet, options);

            // Überprüfen Sie den Kopiervorgang
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // Ergebnis speichern
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


