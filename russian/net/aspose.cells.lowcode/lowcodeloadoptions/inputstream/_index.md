---
title: "LowCodeLoadOptions.InputStream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeLoadOptions. Получает и задает поток шаблона"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

Получает и задаёт поток Stream шаблона.

```csharp
public Stream InputStream { get; set; }
```

### Примечания

При установке ненулевого потока в это свойство, ранее установленное значение для [`InputFile`](../inputfile/) будет игнорироваться.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // Создайте пример данных в поток памяти
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // Создайте параметры загрузки с InputStream
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // Создайте новую книгу, используя поток
                using (Workbook workbook = new Workbook(stream))
                {
                    // Получить доступ к первому листу
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // Продемонстрируйте, что содержимое было загружено
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


