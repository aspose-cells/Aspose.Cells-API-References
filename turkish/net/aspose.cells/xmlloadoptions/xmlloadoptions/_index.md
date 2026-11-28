---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions yapıcı. XML dosyasını yükleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

XML dosyası yükleme seçeneklerini temsil eder

```csharp
public XmlLoadOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni XML yükleme seçenekleri oluşturun
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Sayısal veya tarih değerlerini dönüştürmek için ayarlayın
            options.ConvertNumericOrDate = true;
            
            // Seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook("input.xml", options);
            
            // Hücre verilerine erişin
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // Çalışma kitabını kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

XML dosyası yükleme seçeneklerini temsil eder

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | LoadFormat | Yükleme formatı türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // LoadFormat parametresiyle XmlLoadOptions örneği oluşturun
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // XmlLoadOptions'ın bazı özelliklerini ayarlayın
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Yükleme seçeneklerini kullanarak bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];

                // Bazı bilgileri gösterin
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Çalışma kitabını kaydedin
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


