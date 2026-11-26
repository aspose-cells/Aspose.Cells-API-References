---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptions. Получает и задает поток Stream для записи сгенерированных данных. При установке этого свойства значением, отличным от null, OutputFile будет игнорироваться"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

Получает и задает поток Stream для записи сгенерированных данных. При установке этого свойства значением, отличным от null, [`OutputFile`](../outputfile/) будет игнорироваться.

```csharp
public Stream OutputStream { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class LowCodeSaveOptionsPropertyOutputStreamDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // Создать экземпляр LowCodeSaveOptions
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // Создать поток памяти для демонстрации
                using (MemoryStream stream = new MemoryStream())
                {
                    // Установить свойство OutputStream
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // Сохранить, используя параметры (будет записано в наш поток памяти)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // Проверить, что поток был записан
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // Создать новую книгу из потока, чтобы проверить содержимое
                    Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
                    Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


