---
title: "OoxmlSaveOptions.EmbedOoxmlAsOleObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OoxmlSaveOptions özelliği. OleObject'in Ooxml dosyalarını ole nesne olarak gömüp gömmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

OleObject'in Ooxml dosyalarını ole nesne olarak gömüp gömmeyeceğini gösterir.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Açıklamalar

Yalnızca OleObject için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
            
            // OOXML kaydetme seçeneklerini oluştur ve EmbedOoxmlAsOleObject'i ayarla
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
        }
    }
}
```

### Ayrıca Bakınız

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


