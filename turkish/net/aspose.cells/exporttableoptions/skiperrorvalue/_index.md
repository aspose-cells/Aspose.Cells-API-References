---
title: "ExportTableOptions.SkipErrorValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions özelliği. Sütun için geçersiz değerin atlanıp atlanmayacağını gösterir. Örneğin sütun tipi ondalık ise değer decimal.MaxValue'dan büyük olduğunda ve bu özellik true ise, tekrar istisna fırlatmayacağız. Varsayılan değer false'dur."
type: docs
url: /tr/net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

Sütun için geçersiz değerin atlanıp atlanmayacağını gösterir. Örneğin, sütun tipi decimal ise ve değer decimal.MaxValue'dan büyükse ve bu özellik true ise, tekrar istisna fırlatmayacağız. Varsayılan değer false'tur.

```csharp
public bool SkipErrorValue { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertySkipErrorValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;

            Worksheet ws = wb.Worksheets[0];

            // İlk test durumu - sayısal değerler
            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[0][0] is string)); // Should be False
            Console.WriteLine("Value: " + data.Rows[0][0]); // Should be 1.56

            // İkinci test durumu - karışık değerler
            ws.Cells["A2"].Value = "dummy";
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"

            // Üçüncü test durumu - dize olarak dışa aktar
            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);
            Console.WriteLine("Is string: " + (data.Rows[1][0] is string)); // Should be True
            Console.WriteLine("Value: " + data.Rows[1][0]); // Should be "1,56"
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


