---
title: "Sınıf FormulaParseOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FormulaParseOptions sınıfı. Formül ayrıştırılırken seçenekleri temsil eder"
type: docs
url: /tr/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

Formül ayrıştırılırken seçenekleri temsil eder.

```csharp
public class FormulaParseOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Mevcut çalışma kitabının mevcut dış bağlantılarında dış bağlantı olmadan kullanıcı tanımlı işlev için eklentileri kontrol edip etmeyeceği. Varsayılan değer true'tır (eğer kullanıcı tanımlı işlev mevcut dış bağlantılardaki bir eklentiyle eşleşirse, o eklenti olarak alınır). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Özel işlevlerin ayrıştırılması için tanım. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Formülün yerel formatta olup olmadığı. Varsayılan değer false'tur. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Verilen formülün ayrıştırılıp ayrıştırılmayacağı. Varsayılan değer true'tır. False ise, verilen formül dizesi hücrede olduğu gibi tutulur ve kullanıcı diğer yöntemleri çağırana kadar ya da formül hesaplamaları gibi diğer işlemler ayrıştırılmış formül verisine ihtiyaç duyana kadar. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Formülün R1C1 referans stilinde olup olmadığı. Varsayılan değer false'tur. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // FormulaParseOptions örneği oluştur
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Seçenekleri kullanarak bir hücreye formül ekle
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Çalışma kitabını kaydedin
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


