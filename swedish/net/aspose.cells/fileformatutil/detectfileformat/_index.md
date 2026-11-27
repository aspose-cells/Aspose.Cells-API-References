---
title: "FileFormatUtil.DetectFileFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Upptäcker och returnerar information om formatet för en Excel som lagras i en ström"
type: docs
url: /sv/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Detekterar och returnerar information om ett Excel-format som lagras i en ström.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström |  |

### Returvärde

Ett [`FileFormatInfo`](../../fileformatinfo/)‑objekt som innehåller den upptäckta informationen.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Förbered en MemoryStream med arbetsbokens data
            using (MemoryStream stream = new MemoryStream())
            {
                // Spara arbetsboken till ström i XLSX‑format
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // Detektera filformat från ström
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // Visa detekteringsresultat
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // Spara den ursprungliga arbetsboken för verifiering
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### Se även

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Detekterar och returnerar information om ett Excel-format som lagras i en ström.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström |  |
| lösenord | String | Lösenordet för krypterade ooxml‑filer. |

### Returvärde

Ett [`FileFormatInfo`](../../fileformatinfo/)‑objekt som innehåller den upptäckta informationen.

### Exempel

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

### Se även

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Detekterar och returnerar information om ett Excel-format som lagras i en fil.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filens sökväg. |

### Returvärde

Ett [`FileFormatInfo`](../../fileformatinfo/)‑objekt som innehåller den upptäckta informationen.

### Anmärkningar

Stöder endast kontroll av vissa filer med magisk signatur. Om det inte finns någon magisk signatur kan vi inte exakt upptäcka filformatet.

### Exempel

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

### Se även

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Detekterar och returnerar information om ett Excel-format som lagras i en fil.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | String | Filens sökväg. |
| lösenord | String | Lösenordet för krypterade ooxml‑filer. |

### Returvärde

Ett [`FileFormatInfo`](../../fileformatinfo/)‑objekt som innehåller den upptäckta informationen.

### Anmärkningar

Stöder endast kontroll av vissa filer med magisk signatur. Om det inte finns någon magisk signatur kan vi inte exakt upptäcka filformatet.

### Exempel

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
            
            // Detektera XLSX‑filformat
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // Detektera DOCX‑filformat
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### Se även

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


