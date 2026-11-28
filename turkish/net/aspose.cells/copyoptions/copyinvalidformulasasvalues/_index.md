---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions özelliği. Formül hedef için geçerli değilse yalnızca değerleri kopyala"
type: docs
url: /tr/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

Formül hedef konum için geçerli değilse, yalnızca değerleri kopyalar.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma sayfası içeren bir kaynak çalışma kitabı oluşturun
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Bazı bağlamlarda geçersiz olabilecek bir formül ekleyin
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // Bir hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            
            // Geçersiz formülleri değerlere dönüştürmek için kopyalama seçeneklerini ayarlayın
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // Seçeneklerle çalışma sayfasını kopyalayın
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // Sonuçları doğrulayın
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


