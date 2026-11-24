---
title: "SheetSet.SheetSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetSet-Konstruktor. Erstellt ein Blattset basierend auf genauen Blattindizes"
type: docs
url: /de/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

Erstellt ein Blattset basierend auf genauen Blattindizes.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndexes | Int32[] | nullbasierte Blattindizes. |

### Hinweise

Wenn ein Blatt gefunden wird, das nicht in der Arbeitsmappe ist, wird während des Renderns eine Ausnahme ausgelöst.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit 3 Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Identifikationstext zu jedem Blatt hinzufügen
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // SheetSet mit spezifischen Blattindizes (0 und 2) erstellen
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // PDF-Speicheroptionen mit unserem Blattset erstellen
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // Arbeitsmappe mit ausgewählten Blättern speichern
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

Erstellt ein Blattset basierend auf genauen Blattnamen.

```csharp
public SheetSet(params string[] sheetNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetNames | String[] | Blattnamen. |

### Hinweise

Wenn ein Blatt gefunden wird, das nicht in der Arbeitsmappe ist, wird während des Renderns eine Ausnahme ausgelöst.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // Eine neue Arbeitsmappe erstellen und Blätter hinzufügen
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // Blattnamen für SheetSet vorbereiten
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // SheetSet mit String-Array-Parameter erstellen
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // PDF-Speicheroptionen mit erstellt­em SheetSet konfigurieren
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // Arbeitsmappe mit angegebenen Blättern als PDF speichern
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


