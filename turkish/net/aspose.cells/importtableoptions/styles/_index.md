---
title: "ImportTableOptions.Styles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Tablonun her sütunu için stilleri alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

Tablonun her sütunu için stilleri alır ve ayarlar.

```csharp
public Style[] Styles { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyStylesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri tablosu oluştur
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // ImportTableOptions oluştur ve Styles özelliğini ayarla
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // Her sütun için stiller oluştur
                Style[] columnStyles = new Style[2];

                // Ürün sütunu için stil (kalın, mavi yazı tipi)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Fiyat sütunu için stil (para birimi formatı, yeşil yazı tipi)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // Styles özelliğini ayarla
                options.Styles = columnStyles;

                // Stillerle veri içe aktar
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // Uygulanan stilleri göster
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // Çalışma kitabını kaydedin
                workbook.Save("StylesDemo.xlsx");
                Console.WriteLine("Workbook saved with styled data.");
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

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


