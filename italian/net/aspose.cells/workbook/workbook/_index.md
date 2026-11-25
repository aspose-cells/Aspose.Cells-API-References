---
title: "Workbook.Workbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore Workbook. Inizializza una nuova istanza della classe Workbook"
type: docs
url: /it/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Inizializza una nuova istanza della classe [`Workbook`](../).

```csharp
public Workbook()
```

### Osservazioni

Il tipo di formato file predefinito è Xlsx. Se desideri creare altri tipi di file, utilizza Workbook(FileFormatType).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro usando il costruttore
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Salva la cartella di lavoro
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Inizializza una nuova istanza della classe [`Workbook`](../).

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileFormatType | FileFormatType | Il nuovo formato file. |

### Osservazioni

Il tipo di formato file predefinito è Excel97To2003.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con formato file XLSX
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci alcuni dati nella cella A1
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

Inizializza una nuova istanza vuota della classe [`Workbook`](../) con opzioni

```csharp
public Workbook(LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LoadOptions | Le opzioni. |

### Vedi anche

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

Inizializza una nuova istanza della classe [`Workbook`](../) e apre un file.

```csharp
public Workbook(string file)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | String | Il nome del file. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Il percorso della directory dei documenti.
            string dataDir = "Your Document Directory";

            // Crea un Workbook da un file Excel esistente
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Visualizza alcune informazioni sul foglio di lavoro
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // Salva il workbook in formato MHTML
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // Crea un altro Workbook dal file MHTML salvato
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

Inizializza una nuova istanza della classe [`Workbook`](../) e apre uno stream.

```csharp
public Workbook(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Lo stream. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // Crea un file Excel di esempio in memoria
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // Crea una nuova istanza di Workbook usando il costruttore Stream
                Workbook workbook = new Workbook(sampleStream);

                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];

                // Visualizza i dati caricati
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // Salva la cartella di lavoro in un file
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

Inizializza una nuova istanza della classe [`Workbook`](../) e apre un file.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | String | Il nome del file. |
| loadOptions | LoadOptions | Le opzioni di caricamento |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento senza LightCellsDataHandler
            LoadOptions loadOptions = new LoadOptions();

            // Inizializza il workbook con il percorso del file e le opzioni di caricamento
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Dimostra che il workbook è caricato accedendo al conteggio dei fogli di lavoro
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

Inizializza una nuova istanza della classe [`Workbook`](../) e apre uno stream.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Lo stream. |
| loadOptions | LoadOptions | Le opzioni di caricamento |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un file Excel di esempio in memoria
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // Crea LoadOptions con impostazioni specifiche
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // Crea un'istanza di Workbook usando il #ctor con Stream e LoadOptions
                Workbook workbook = new Workbook(stream, loadOptions);

                // Visualizza le informazioni di base sul workbook caricato
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // Mostra il contenuto di alcune celle se disponibile
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // Crea un semplice file Excel in memoria per la dimostrazione
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


