---
title: "FormulaParseOptions.CheckAddIn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaParseOptions özelliği. Kullanıcı tanımlı işlevin dış bağlantısı olmadan, mevcut çalışma kitabının dış bağlantılarındaki eklentileri kontrol edip etmeyeceğini belirler. Varsayılan değer true'tir; kullanıcı tanımlı işlev mevcut dış bağlantılardaki bir eklentiyle eşleşirse, onu eklenti olarak alır."
type: docs
url: /tr/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Mevcut çalışma kitabının mevcut dış bağlantılarında dış bağlantı olmadan kullanıcı tanımlı işlev için eklentileri kontrol edip etmeyeceği. Varsayılan değer true'tır (eğer kullanıcı tanımlı işlev mevcut dış bağlantılardaki bir eklentiyle eşleşirse, o eklenti olarak alınır).

```csharp
public bool CheckAddIn { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Eklenti işlevi kaydet
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // CheckAddIn=false olmadan - formül eklenti formatına dönüştürülecek
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // CheckAddIn=false ile - formül değişmeden kalır
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


