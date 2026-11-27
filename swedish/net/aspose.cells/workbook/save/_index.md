---
title: "Workbook.Save"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Sparar arbetsboken till disken."
type: docs
url: /sv/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Sparar arbetsboken till disken.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Filnamnet. |
| saveFormat | SaveFormat | Spara formattypen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet och lägg till exempeldata.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Spara arbetsboken i XLSX-format.
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Spara arbetsboken i PDF-format.
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Spara arbetsboken till disken.

```csharp
public void Save(string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Spara arbetsboken i olika format med strängparameter.
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Sparar arbetsboken till disken.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Filnamnet. |
| saveOptions | SaveOptions | Sparalternativen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Öppna det första kalkylbladet och lägg till data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Skapa HTML-sparalternativ och konfigurera dem
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Spara arbetsboken med alternativ
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### Se även

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Sparar arbetsboken till strömmen.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Filströmmen. |
| saveFormat | SaveFormat | Sparfilformatstypen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet och lägg till exempeldata.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Skapa en minnesström för att spara arbetsboken
                using (MemoryStream stream = new MemoryStream())
                {
                    // Spara arbetsboken till strömmen i XLSX-format
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Visa framgångsmeddelande
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Återställ strömmens position för eventuell vidare bearbetning
                    stream.Position = 0;

                    // Spara eventuellt till fil för verifiering
                    using (FileStream fileStream = File.Create("StreamSaveDemo.xlsx"))
                    {
                        stream.CopyTo(fileStream);
                    }
                    Console.WriteLine("Stream content also saved to file: StreamSaveDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook to stream: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Sparar arbetsboken till strömmen.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Filströmmen. |
| saveOptions | SaveOptions | Sparalternativen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Öppna det första kalkylbladet och lägg till data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Skapa en MemoryStream för att spara arbetsboken
            MemoryStream stream = new MemoryStream();

            try
            {
                // Skapa SaveOptions för PDF-format
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Spara arbetsboken till strömmen med de angivna alternativen
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // Återställ strömmens position för eventuell vidare användning
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Rensa resurser
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### Se även

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Skapar resultatspridarket och överför det till klienten för att sedan öppna det i webbläsaren eller MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| response | HttpResponse | Response-objekt för att returnera kalkylbladet till klienten. |
| fileName | String | Namnet på den skapade filen. |
| contentDisposition | ContentDisposition | Innehållsdispositionstypen. |
| saveOptions | SaveOptions | Sparalternativen. |

### Anmärkningar

Denna metod är endast tillgänglig för net4.x-versioner.

### Se även

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Skapar resultatspridarket och överför det till klienten för att sedan öppna det i webbläsaren eller MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| response | HttpResponse | Response-objekt för att returnera kalkylbladet till klienten. |
| fileName | String | Namnet på den skapade filen. |
| contentDisposition | ContentDisposition | Innehållsdispositionstypen. |
| saveOptions | SaveOptions | Sparalternativen. |
| enableHttpCompression | Boolean | om HTTP-komprimering ska användas |

### Anmärkningar

Denna metod är endast tillgänglig för net4.x-versioner.

### Se även

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


