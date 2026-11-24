---
title: "Workbook.Combine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Kombiniert ein weiteres Workbook-Objekt"
type: docs
url: /de/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Kombiniert ein weiteres Workbook‑Objekt.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| secondWorkbook | Arbeitsmappe | Ein weiteres Workbook-Objekt. |

### Hinweise

Excel-, ODS‑, CSV‑ und andere Dateien zu einer Datei zusammenführen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // Quell‑Workbook erstellen
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // Workbooks kombinieren
            destWorkbook.Combine(sourceWorkbook);

            // Save the combined workbook
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


