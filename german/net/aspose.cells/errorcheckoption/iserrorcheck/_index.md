---
title: "ErrorCheckOption.IsErrorCheck"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorCheckOption-Methode. Prüft, ob der angegebene Fehlertyp überprüft wird"
type: docs
url: /de/net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

Prüft, ob der angegebene Fehlertyp überprüft wird.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | Fehlertyp kann überprüft werden |

### Rückgabewert

gibt true zurück, wenn der angegebene Fehlertyp überprüft wird (grünes Dreieck wird für die Zelle angezeigt, wenn die Prüfung fehlgeschlagen ist).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            int index = options.Add();
            ErrorCheckOption option = options[index];

            // Fehlerprüfungseinstellungen konfigurieren
            option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
            option.SetErrorCheck(ErrorCheckType.InconsistRange, false);

            // Bereich hinzufügen, um diese Einstellungen anzuwenden
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 10;
            area.StartColumn = 0;
            area.EndColumn = 5;
            option.AddRange(area);

            // Einstellungen überprüfen und anzeigen
            Console.WriteLine("NumberStoredAsText check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
            Console.WriteLine("EvaluationError check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.EvaluationError));
            Console.WriteLine("InconsistRange check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.InconsistRange));
        }
    }
}
```

### Siehe auch

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


