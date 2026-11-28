---
title: "AbstractTextLoadOptions.Encoding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractTextLoadOptions özelliği. Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir"
type: docs
url: /tr/net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir.

```csharp
public Encoding Encoding { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // ASCII kodlamasında örnek CSV verisi oluşturun
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);

            // ASCII kodlaması belirtilerek çalışma kitabını yükleyin
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            Cells cells = wb.Worksheets[0].Cells;

            // Yüklenen verileri gösterin
            Console.WriteLine($"A1: {cells[0, 0].StringValue}");
            Console.WriteLine($"B1: {cells[0, 1].StringValue}");
            Console.WriteLine($"A2: {cells[1, 0].StringValue}");
            Console.WriteLine($"B2: {cells[1, 1].IntValue}");

            // Bazı Unicode metinler ekleyin
            cells[2, 0].PutValue("日本語のテキスト");
            
            // UTF-8 kodlamasıyla kaydet
            MemoryStream outputStream = new MemoryStream();
            wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
            
            // UTF-8 BOM'u göstermek için ilk birkaç baytı görüntüle
            byte[] outputBytes = outputStream.ToArray();
            Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


