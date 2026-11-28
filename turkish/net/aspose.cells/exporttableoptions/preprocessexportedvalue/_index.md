---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions yöntemi. Dışa aktarılacak mevcut hücrenin değerini ön işleme tabi tut"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Dışa aktarılacak mevcut hücrenin değerini ön işleme tabi tut.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellRow | Int32 | geçerli hücrenin satır indeksi |
| cellColumn | Int32 | hücrenin sütun indeksi |
| değer | CellValue | geçerli hücrenin değeri ve türü |

### Dönüş Değeri

Geçerli hücrenin farklı bir tür ve/veya değerle değiştirilip değiştirilmediği.

### Açıklamalar

Satır ve sütun indeksi, hücrenin çalışma sayfasındaki mutlak indeksidir, dışa aktarılan tablodaki indeks değildir. Kullanıcı, bu yöntemin geçersiz kılma uygulamasında geçerli hücrenin değerini kontrol edebilir; eğer geçerli hücrenin başka bir tür ve değerle değiştirilmesi gerekiyorsa, burada uygulama beklenen tür ve değeri CellValue nesnesine ayarlamalı ve true döndürmelidir. Varsayılan olarak bu yöntem hiçbir şey yapmaz ve false döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasında örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // ExportTableOptions bir örnek oluşturun
            ExportTableOptions exportOptions = new ExportTableOptions();

            // Demonstrasyon için bir CellValue nesnesi oluşturun
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // PreprocessExportedValue yöntemini belirli parametrelerle (satır 0, sütun 0, CellValue) çağırın
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // Yöntem çağrısının sonucunu gösterin
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // Gerekirse hücreyi işlenmiş değerle değiştirin
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


