---
title: "Klasse LowCodeSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodeSaveOptions Klasse. Optionen zum Speichern generierter Ergebnisse auf Low-Code-Weise"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

Optionen zum Speichern generierter Ergebnisse in Low‑Code‑Manier.

```csharp
public class LowCodeSaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Liest und setzt die Datei (mit Pfad falls nötig) zum Speichern der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird [`OutputStream`](./outputstream/) ignoriert. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Liest und setzt den Stream, in den die generierten Daten geschrieben werden. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird [`OutputFile`](./outputfile/) ignoriert. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Liest und setzt das Speicherformat für die Ausgabe. Im Allgemeinen sind für einen bestimmten Prozess auf Low-Code-Weise nur einige spezifische Formate zulässig. Bitte geben Sie das korrekte Format für den jeweiligen Prozess an, sonst kann ein unerwartetes Ergebnis oder sogar eine Ausnahme auftreten. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein Arbeitsblatt hinzu und füge einige Daten ein
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Erstelle Speicheroptionen
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // Speichere das Arbeitsbuch mit den angegebenen Optionen
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


