---
title: "Sınıf OdsCellField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OdsCellField sınıfı. ODS'nin hücre alanını temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

ods'nin hücre alanını temsil eder.

```csharp
public class OdsCellField
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Hücrenin sütun indeksini alır ve ayarlar. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Alan değerinin özel biçimini temsil eder. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Alan tipini alır ve ayarlar. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Hücrenin satır indeksini alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Koleksiyon aracılığıyla bir OdsCellField oluşturun (parametresiz ctor yok)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Az önce eklediğimiz alanı alın
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // OdsCellField ile tanımlanan hücreye bir şeyler yazın
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Koleksiyon kullanımını göstermek için aynı alanı tekrar ekleyin (isteğe bağlı)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Tüm ODS alanlarını güncelleyerek kaydedilen dosyada yansıtılmalarını sağlayın
                odsFields.UpdateFieldsValue();

                // Özellik değerlerini konsola gösterin
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Çalışma kitabını ODS dosyası olarak kaydedin
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


