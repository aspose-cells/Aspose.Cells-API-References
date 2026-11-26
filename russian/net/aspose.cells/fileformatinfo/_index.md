---
title: "Класс FileFormatInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FileFormatInfo. Содержит данные, возвращаемые методами обнаружения формата файлов FileFormatUtil"
type: docs
url: /ru/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

Содержит данные, возвращаемые методами обнаружения формата файлов [`FileFormatUtil`](../fileformatutil/).

```csharp
public class FileFormatInfo
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Получает обнаруженный формат файла. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Возвращает true, если документ зашифрован и требует пароль для открытия. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Указывает, защищён ли файл сервером Microsoft Rights Management. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Получает обнаруженный формат загрузки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // Загрузите пример файла, чтобы определить его формат
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Отобразить информацию о формате файла
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // Сохранить информацию в текстовый файл
            string outputFilePath = "FileFormatInfo.txt";
            using (System.IO.StreamWriter writer = new System.IO.StreamWriter(outputFilePath))
            {
                writer.WriteLine("File Format Information:");
                writer.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
                writer.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
                writer.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
                writer.WriteLine($"Load Format: {fileInfo.LoadFormat}");
            }

            Console.WriteLine($"File format information saved to {outputFilePath}");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


