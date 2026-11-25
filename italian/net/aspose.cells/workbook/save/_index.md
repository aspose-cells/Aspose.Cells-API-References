---
title: "Workbook.Save"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Salva la cartella di lavoro su disco"
type: docs
url: /it/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Salva la cartella di lavoro su disco.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome del file. |
| saveFormat | SaveFormat | Il tipo di formato di salvataggio. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Salva la cartella di lavoro in formato XLSX
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Salva la cartella di lavoro in formato PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Salva la cartella di lavoro su disco.

```csharp
public void Save(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String |  |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Salva la cartella di lavoro in formati diversi usando il parametro stringa
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Salva la cartella di lavoro su disco.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | Il nome del file. |
| saveOptions | SaveOptions | Le opzioni di salvataggio. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Crea le opzioni di salvataggio HTML e configurale
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Salva la cartella di lavoro con le opzioni
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Salva la cartella di lavoro sullo stream.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di file. |
| saveFormat | SaveFormat | Il tipo di formato di file di salvataggio. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Crea un flusso di memoria per salvare la cartella di lavoro
                using (MemoryStream stream = new MemoryStream())
                {
                    // Salva la cartella di lavoro nel flusso in formato XLSX
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Visualizza il messaggio di successo
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Reimposta la posizione del flusso per un eventuale ulteriore elaborazione
                    stream.Position = 0;

                    // Facoltativamente salva su file per verifica
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

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Salva la cartella di lavoro sullo stream.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso di file. |
| saveOptions | SaveOptions | Le opzioni di salvataggio. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro e aggiungi alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Crea un MemoryStream per salvare la cartella di lavoro
            MemoryStream stream = new MemoryStream();

            try
            {
                // Crea SaveOptions per il formato PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Salva la cartella di lavoro nel flusso con le opzioni specificate
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // Reimposta la posizione del flusso per un eventuale utilizzo successivo
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Pulisci le risorse
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Crea il foglio di calcolo risultato e lo trasferisce al client, quindi lo apre nel browser o in MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| risposta | HttpResponse | Oggetto Response per restituire il foglio di calcolo al client. |
| fileName | String | Il nome del file creato. |
| contentDisposition | ContentDisposition | Il tipo di disposizione del contenuto. |
| saveOptions | SaveOptions | Le opzioni di salvataggio. |

### Osservazioni

Questo metodo è disponibile solo per le versioni net4.x.

### Vedi anche

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Crea il foglio di calcolo risultato e lo trasferisce al client, quindi lo apre nel browser o in MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| risposta | HttpResponse | Oggetto Response per restituire il foglio di calcolo al client. |
| fileName | String | Il nome del file creato. |
| contentDisposition | ContentDisposition | Il tipo di disposizione del contenuto. |
| saveOptions | SaveOptions | Le opzioni di salvataggio. |
| enableHttpCompression | Booleano | se la compressione http deve essere utilizzata |

### Osservazioni

Questo metodo è disponibile solo per le versioni net4.x.

### Vedi anche

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


