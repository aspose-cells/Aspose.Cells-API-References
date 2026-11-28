---
title: "TableStyle.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableStyle özelliği. Tablo stilinin adını alır"
type: docs
url: /tr/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Tablo stilinin adını alır.

```csharp
public string Name { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Tablo stilleri koleksiyonuna eriş
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Koleksiyondan ilk tablo stilini al
                TableStyle tableStyle = tableStyles[0];

                // Name özelliğinin değerini göster
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Salt okunur özelliğe erişimi göster
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Stili referans almak için adı kullanabileceğimizi göster
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Çalışma kitabını kaydedin
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


