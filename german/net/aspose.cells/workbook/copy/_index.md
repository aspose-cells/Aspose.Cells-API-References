---
title: "Workbook.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Kopiert ein anderes Workbook-Objekt"
type: docs
url: /de/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Kopiert ein weiteres Workbook‑Objekt.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Arbeitsmappe | Quell-Workbook-Objekt. |
| copyOptions | CopyOptions | Die Optionen zum Kopieren eines anderen Workbooks. |

### Hinweise

Es ist sehr einfach, eine Excel-Datei zu klonen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // Quell-Workbook mit Makros
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // Ziel-Workbook (leer oder bereits vorhanden)
            Workbook destWorkbook = new Workbook();
            
            // Kopieroptionen konfigurieren, um Makros zu behalten
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // Inhalte vom Quell- zum Ziel-Workbook kopieren
            sourceWorkbook.Copy(destWorkbook, options);
            
            // Ergebnis speichern
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Kopiert Daten aus einem Quell‑Workbook‑Objekt.

```csharp
public void Copy(Workbook source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Arbeitsmappe | Quell-Workbook-Objekt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // Quell- und Ausgabedateipfade
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // Lade die Quellarbeitsmappe
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // Ein neues Workbook erstellen und Inhalte aus der Quelle kopieren
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // Das kopierte Workbook speichern
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


