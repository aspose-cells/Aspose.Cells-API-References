---
title: "LowCodeLoadOptions.InputFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeLoadOptions özelliği. Şablonun gerekirse dosya yolu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

Şablonun dosyasını (gerekirse yol ile) alır ve ayarlar.

```csharp
public string InputFile { get; set; }
```

### Açıklamalar

Bu özelliğe null olmayan ve boş olmayan bir yol ayarlandığında, daha önce ayarlanan [`InputStream`](../inputstream/) değeri göz ardı edilecektir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // Örnek bir şablon dosyası oluşturun ve kaydedin
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // LowCodeLoadOptions başlatın ve InputFile özelliğini gösterin
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // Şablonumuzu kullanmak için InputFile özelliğini ayarlayın
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // Belirtilen şablon dosyasını kullanarak çalışma kitabını yükleyin
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // Yüklenen şablonu değiştirin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


