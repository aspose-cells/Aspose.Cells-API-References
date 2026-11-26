---
title: "FileFormatUtil.DetectFileFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Обнаруживает и возвращает информацию о формате Excel, хранящегося в потоке"
type: docs
url: /ru/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Определяет и возвращает информацию о формате Excel, хранящегося в потоке.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream |  |

### Возвращаемое значение

Объект [`FileFormatInfo`](../../fileformatinfo/), содержащий обнаруженную информацию.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Подготовьте MemoryStream с данными книги.
            using (MemoryStream stream = new MemoryStream())
            {
                // Сохранить книгу в поток в формате XLSX.
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // Определить формат файла из потока.
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // Отобразить результаты определения.
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // Сохранить оригинальную книгу для проверки.
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### См. также

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Определяет и возвращает информацию о формате Excel, хранящегося в потоке.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream |  |
| пароль | String | Пароль для зашифрованных файлов ooxml. |

### Возвращаемое значение

Объект [`FileFormatInfo`](../../fileformatinfo/), содержащий обнаруженную информацию.

### Примеры

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

### См. также

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Определяет и возвращает информацию о формате Excel, хранящегося в файле.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |

### Возвращаемое значение

Объект [`FileFormatInfo`](../../fileformatinfo/), содержащий обнаруженную информацию.

### Примечания

Поддерживает только проверку некоторых файлов по магической подписи. Если магической подписи нет, мы не можем точно определить формат файла.

### Примеры

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

### См. также

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Определяет и возвращает информацию о формате Excel, хранящегося в файле.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| пароль | String | Пароль для зашифрованных файлов ooxml. |

### Возвращаемое значение

Объект [`FileFormatInfo`](../../fileformatinfo/), содержащий обнаруженную информацию.

### Примечания

Поддерживает только проверку некоторых файлов по магической подписи. Если магической подписи нет, мы не можем точно определить формат файла.

### Примеры

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
            
            // Определить формат файла XLSX.
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // Определить формат файла DOCX.
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### См. также

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


