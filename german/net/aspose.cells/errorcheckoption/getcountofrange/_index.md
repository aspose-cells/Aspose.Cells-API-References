---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorCheckOption-Methode. Gibt die Anzahl der Bereiche zurück, die von dieser Einstellung beeinflusst werden"
type: docs
url: /de/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Ermittelt die Anzahl der von dieser Einstellung beeinflussten Bereiche.

```csharp
public int GetCountOfRange()
```

### Rückgabewert

die Anzahl der Bereiche, die von dieser Einstellung beeinflusst werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fehlerprüfungsoptionssammlung abrufen
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // Erste Fehlerprüfungsoption hinzufügen
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // Zweite Fehlerprüfungsoption hinzufügen
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // Demonstriere die GetCountOfRange-Methode
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


