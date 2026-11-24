---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EbookLoadOptions-Konstruktor. Erstellt eine Option zum Laden der Ebook-Datei"
type: docs
url: /de/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

Erstellt eine Option zum Laden der Ebook-Datei.

```csharp
public EbookLoadOptions()
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von EbookLoadOptions mithilfe des Konstruktors
            EbookLoadOptions options = new EbookLoadOptions();

            // Einige grundlegende Eigenschaften festlegen
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Lade eine Ebook-Datei mit den angegebenen Optionen
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Als Excel-Datei speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

Erstellt eine Option für das Laden der Ebook-Datei.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | LoadFormat | Das Ladeformat |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine EbookLoadOptions-Instanz mit dem LoadFormat-Parameter
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Bestätigung anzeigen
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Beispielhafte Verwendung: Lade ein Arbeitsbuch mit diesen Optionen
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Ergebnis speichern
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


