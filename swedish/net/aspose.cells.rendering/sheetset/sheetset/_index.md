---
title: "SheetSet.SheetSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetSet-konstruktor. Skapar en bladuppsättning baserad på exakta bladindex"
type: docs
url: /sv/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

Skapar en bladuppsättning baserad på exakta bladindex.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndexes | Int32[] | nollbaserade bladindex. |

### Anmärkningar

Om ett blad påträffas som inte finns i arbetsboken kastas ett undantag under rendering.

### Exempel

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
            // Skapa en ny arbetsbok med 3 blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Lägg till identifieringstext till varje blad
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // Skapa SheetSet med specifika bladindex (0 och 2)
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // Skapa PDF-sparalternativ med vår bladuppsättning
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // Spara arbetsboken med valda blad
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

### Se även

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

Skapar en bladuppsättning baserad på exakta bladnamn.

```csharp
public SheetSet(params string[] sheetNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetNames | String[] | bladnamn. |

### Anmärkningar

Om ett blad påträffas som inte finns i arbetsboken kastas ett undantag under rendering.

### Exempel

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
            // Skapa en ny arbetsbok och lägg till blad
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // Förbered bladnamn för SheetSet
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // Skapa SheetSet med strängarrayparameter
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // Konfigurera PDF-sparalternativ med skapad SheetSet
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // Spara arbetsbok till PDF med angivna blad
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

### Se även

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


