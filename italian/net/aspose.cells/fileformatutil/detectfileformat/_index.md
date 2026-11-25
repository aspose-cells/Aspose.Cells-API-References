---
title: "FileFormatUtil.DetectFileFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Rileva e restituisce le informazioni sul formato di un Excel memorizzato in uno stream"
type: docs
url: /it/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in uno stream.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream |  |

### Valore di ritorno

Un oggetto [`FileFormatInfo`](../../fileformatinfo/) che contiene le informazioni rilevate.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FileFormatUtilMethodDetectFileFormatWithStreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Prepara un MemoryStream con i dati della cartella di lavoro
            using (MemoryStream stream = new MemoryStream())
            {
                // Salva la cartella di lavoro nello stream in formato XLSX
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // Rileva il formato del file dallo stream
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // Mostra i risultati del rilevamento
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // Salva la cartella di lavoro originale per la verifica
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in uno stream.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream |  |
| password | String | La password per i file ooxml crittografati. |

### Valore di ritorno

Un oggetto [`FileFormatInfo`](../../fileformatinfo/) che contiene le informazioni rilevate.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStreamStringDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xlsx";
            
            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
                Console.WriteLine("Is password valid: " + FileFormatUtil.VerifyPassword(stream, "test"));
            }

            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
            }
        }
    }
}
```

### Vedi anche

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in un file.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |

### Valore di ritorno

Un oggetto [`FileFormatInfo`](../../fileformatinfo/) che contiene le informazioni rilevate.

### Osservazioni

Supporta solo il controllo di alcuni file con firma magica. Se non c'è firma magica, non possiamo rilevare con precisione il formato del file.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            
            Console.WriteLine("Load Format: " + info.LoadFormat);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(info.FileFormatType);
            LoadFormat loadFormat = FileFormatUtil.SaveFormatToLoadFormat(saveFormat);
            
            Console.WriteLine("Save Format: " + saveFormat);
            Console.WriteLine("Load Format (converted): " + loadFormat);
        }
    }
}
```

### Vedi anche

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in un file.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | String | Il percorso del file. |
| password | String | La password per i file ooxml crittografati. |

### Valore di ritorno

Un oggetto [`FileFormatInfo`](../../fileformatinfo/) che contiene le informazioni rilevate.

### Osservazioni

Supporta solo il controllo di alcuni file con firma magica. Se non c'è firma magica, non possiamo rilevare con precisione il formato del file.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringStringDemo
    {
        public static void Run()
        {
            string sourcePath = @"..\..\..\Data\";
            
            // Rileva il formato del file XLSX
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // Rileva il formato del file DOCX
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### Vedi anche

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


