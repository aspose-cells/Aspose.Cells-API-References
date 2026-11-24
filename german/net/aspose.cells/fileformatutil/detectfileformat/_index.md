---
title: "FileFormatUtil.DetectFileFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatUtil-Methode. Erkennt und gibt die Informationen über ein Excel-Format zurück, das in einem Stream gespeichert ist"
type: docs
url: /de/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Erkennt und gibt die Informationen über das Format einer in einem Stream gespeicherten Excel-Datei zurück.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream |  |

### Rückgabewert

Ein [`FileFormatInfo`](../../fileformatinfo/) Objekt, das die erkannten Informationen enthält.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle einen MemoryStream mit Arbeitsmappendaten
            using (MemoryStream stream = new MemoryStream())
            {
                // Speichere die Arbeitsmappe in einen Stream im XLSX-Format
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // Dateiformat aus Stream erkennen
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // Erkennungsergebnisse anzeigen
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // Originale Arbeitsmappe zur Überprüfung speichern
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Erkennt und gibt die Informationen über das Format einer in einem Stream gespeicherten Excel-Datei zurück.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream |  |
| Passwort | String | Das Passwort für verschlüsselte ooxml-Dateien. |

### Rückgabewert

Ein [`FileFormatInfo`](../../fileformatinfo/) Objekt, das die erkannten Informationen enthält.

### Beispiele

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

### Siehe auch

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Erkennt und gibt die Informationen über das Format einer in einer Datei gespeicherten Excel-Datei zurück.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Dateipfad. |

### Rückgabewert

Ein [`FileFormatInfo`](../../fileformatinfo/) Objekt, das die erkannten Informationen enthält.

### Hinweise

Unterstützt nur die Prüfung einiger Dateien mit magischer Signatur. Wenn keine magische Signatur vorhanden ist, können wir das Dateiformat nicht genau erkennen.

### Beispiele

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

### Siehe auch

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Erkennt und gibt die Informationen über das Format einer in einer Datei gespeicherten Excel-Datei zurück.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Der Dateipfad. |
| Passwort | String | Das Passwort für verschlüsselte ooxml-Dateien. |

### Rückgabewert

Ein [`FileFormatInfo`](../../fileformatinfo/) Objekt, das die erkannten Informationen enthält.

### Hinweise

Unterstützt nur die Prüfung einiger Dateien mit magischer Signatur. Wenn keine magische Signatur vorhanden ist, können wir das Dateiformat nicht genau erkennen.

### Beispiele

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
            
            // XLSX-Dateiformat erkennen
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // DOCX-Dateiformat erkennen
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### Siehe auch

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


