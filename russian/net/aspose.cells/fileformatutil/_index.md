---
title: "Класс FileFormatUtil"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FileFormatUtil. Предоставляет вспомогательные методы для преобразования перечислений форматов файлов в строки или расширения файлов и обратно"
type: docs
url: /ru/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

Предоставляет вспомогательные методы для преобразования перечислений форматов файлов в строки или расширения файлов и обратно.

```csharp
public class FileFormatUtil
```

## Методы

| Имя | Описание |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Определяет и возвращает информацию о формате Excel, хранящегося в потоке. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Определяет и возвращает информацию о формате Excel, хранящегося в файле. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Определяет и возвращает информацию о формате Excel, хранящегося в потоке. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Определяет и возвращает информацию о формате Excel, хранящегося в файле. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Преобразует расширение имени файла в значение SaveFormat. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Преобразование формата файла в формат сохранения. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Возвращает true, если расширение равно .xlt, .xltX, .xltm,.ots. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Преобразует перечисленное значение формата загрузки в расширение файла. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Преобразует значение LoadFormat в значение SaveFormat, если это возможно. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Преобразует перечисленное значение формата сохранения в расширение файла. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Преобразует значение SaveFormat в значение LoadFormat, если это возможно. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Определяет и возвращает информацию о формате Excel, хранящегося в потоке. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFileFormatUtilDemo
    {
        public static void Run()
        {
            string filePath = "example.xlt";
            
            // Определить формат файла
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // Проверить формат файла с помощью Workbook
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


