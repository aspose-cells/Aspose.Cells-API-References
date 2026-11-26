---
title: "Workbook.Save"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Сохраняет рабочую книгу на диск"
type: docs
url: /ru/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Сохраняет книгу на диск.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла. |
| saveFormat | SaveFormat | Тип формата сохранения. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу и добавить примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Сохранить рабочую книгу в формате XLSX
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Сохранить рабочую книгу в формате PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Сохранить книгу на диск.

```csharp
public void Save(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String |  |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Сохранить рабочую книгу в разных форматах, используя строковый параметр
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Сохраняет книгу на диск.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя файла. |
| saveOptions | SaveOptions | Параметры сохранения. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу и добавить данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Создать параметры сохранения HTML и настроить их
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Сохранить рабочую книгу с параметрами
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### См. также

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Сохраняет книгу в поток.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток файла. |
| saveFormat | SaveFormat | Тип формата сохраняемого файла. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу и добавить примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Создать поток памяти для сохранения рабочей книги
                using (MemoryStream stream = new MemoryStream())
                {
                    // Сохранить рабочую книгу в поток в формате XLSX
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Отобразить сообщение об успехе
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Сбросить позицию потока для возможной дальнейшей обработки
                    stream.Position = 0;

                    // При необходимости сохранить в файл для проверки
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

### См. также

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Сохраняет книгу в поток.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток файла. |
| saveOptions | SaveOptions | Параметры сохранения. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу и добавить данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Создать MemoryStream для сохранения рабочей книги
            MemoryStream stream = new MemoryStream();

            try
            {
                // Создать SaveOptions для формата PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Сохранить рабочую книгу в поток с указанными параметрами
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // Сбросить позицию потока для потенциального дальнейшего использования
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Очистить ресурсы
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### См. также

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Создаёт результирующую таблицу и передаёт её клиенту, затем открывает в браузере или в MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ответ | HttpResponse | Объект Response для возврата таблицы клиенту. |
| fileName | String | Имя созданного файла. |
| contentDisposition | ContentDisposition | Тип disposition содержимого. |
| saveOptions | SaveOptions | Параметры сохранения. |

### Примечания

Этот метод доступен только для версий net4.x.

### См. также

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Создаёт результирующую таблицу и передаёт её клиенту, затем открывает в браузере или в MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ответ | HttpResponse | Объект Response для возврата таблицы клиенту. |
| fileName | String | Имя созданного файла. |
| contentDisposition | ContentDisposition | Тип disposition содержимого. |
| saveOptions | SaveOptions | Параметры сохранения. |
| enableHttpCompression | Boolean | нужно ли использовать сжатие http |

### Примечания

Этот метод доступен только для версий net4.x.

### См. также

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


