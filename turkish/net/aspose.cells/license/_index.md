---
title: "License sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.License sınıfı. Bileşeni lisanslamak için yöntemler sağlar"
type: docs
url: /tr/net/aspose.cells/license/
---
## License class

Bileşeni lisanslamak için yöntemler sağlar.

```csharp
public class License
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [License](license/)() | Bu sınıfın yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Bileşeni lisanslar. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Bileşeni lisanslar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // License sınıfının bir örneğini oluşturun
            License license = new License();

            // Lisansı bir lisans dosyası adı kullanarak ayarlayın
            license.SetLicense("Aspose.Cells.NET.lic");

            // Alternatif olarak, lisansı bir akış kullanarak ayarlayın
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // Lisanslı Aspose.Cells işlevselliğinin kullanımını göstermek için ek kod
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // Lisansın doğru şekilde uygulandığını doğrulamak için çalışma kitabını kaydedin
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


