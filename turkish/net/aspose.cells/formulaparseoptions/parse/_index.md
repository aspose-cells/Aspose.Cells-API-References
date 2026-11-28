---
title: "FormulaParseOptions.Parse"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaParseOptions özelliği. Verilen formülün ayrıştırılıp ayrıştırılmayacağını belirler. Varsayılan değer true'tır. False olduğunda, verilen formül dizesi hücre için olduğu gibi tutulur; kullanıcı başka yöntemlerle ayrıştırana kadar veya ayrıştırılmış formül verileri, formüllerin hesaplanması gibi diğer işlemler için gerektiğinde."
type: docs
url: /tr/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Verilen formülün ayrıştırılıp ayrıştırılmayacağı. Varsayılan değer true'tır. False ise, verilen formül dizesi hücrede olduğu gibi tutulur ve kullanıcı diğer yöntemleri çağırana kadar ya da formül hesaplamaları gibi diğer işlemler ayrıştırılmış formül verisine ihtiyaç duyana kadar.

```csharp
public bool Parse { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyParseDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Parse=false ile formülleri ayarla (formüller hemen ayrıştırılmaz)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // Formülleri hesapla (ayrıştırma şimdi gerçekleşecek)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


