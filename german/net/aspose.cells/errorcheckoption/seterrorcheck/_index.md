---
title: "ErrorCheckOption.SetErrorCheck"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorCheckOption-Methode. Legt fest, ob der angegebene Fehlertyp geprüft wird"
type: docs
url: /de/net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Legt fest, ob der angegebene Fehlertyp überprüft wird.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | Fehlertyp kann überprüft werden. |
| isCheck | Boolean | true, wenn der angegebene Fehlertyp überprüft werden muss (grünes Dreieck wird für die Zelle angezeigt, wenn die Prüfung fehlgeschlagen ist). |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Sample text for error checking");
            
            // Fehlerprüfungsoptionen konfigurieren
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            
            // Demonstriere SetErrorCheck mit verschiedenen ErrorCheckType-Werten
            errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            
            // Auf das gesamte Arbeitsblatt anwenden
            errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
            
            workbook.Save("ErrorCheckExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


