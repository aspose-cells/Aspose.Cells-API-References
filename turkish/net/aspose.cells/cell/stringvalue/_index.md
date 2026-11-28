---
title: "Cell.StringValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrede bulunan dize değerini alır. Eğer bu hücrenin türü dize ise dize değerini kendisini döndürür. Diğer hücre türleri için, bu hücrenin belirtilen stiliyle biçimlendirilmiş dize değeri döndürülür. Biçimlendirilmiş hücre değeri, bir hücreyi metin olarak kopyaladığınızda Excel'den alabileceğinizle aynı şeydir; örneğin hücreyi metin düzenleyiciye kopyalamak veya csv'ye dışa aktarmak gibi."
type: docs
url: /tr/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Hücrede bulunan string değerini alır. Eğer bu hücrenin tipi string ise, doğrudan string değerini döndürür. Diğer hücre tipleri için, biçimlendirilmiş string değer (bu hücrenin belirtilen stiliyle biçimlendirilmiş) döndürülür. Biçimlendirilmiş hücre değeri, bir hücreyi metin olarak kopyaladığınızda (örneğin hücreyi metin düzenleyicisine kopyalama veya csv'ye dışa aktarma) Excel'den alabileceğiniz değerle aynıdır.

```csharp
public string StringValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bazı değerler ayarla
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // Formülleri hesapla
            workbook.CalculateFormula();

            // StringValue özelliğini göster
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // Hata değeri durumunu göster
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


