---
title: "Enum ExceptionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExceptionType enum. Özel istisna türü kodunu temsil eder"
type: docs
url: /tr/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Özel istisna türü kodunu temsil eder.

```csharp
public enum ExceptionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Chart | `0` | Geçersiz grafik ayarı. |
| DataType | `1` | Geçersiz veri tipi ayarı. |
| DataValidation | `2` | Geçersiz veri doğrulama ayarı. |
| ConditionalFormatting | `3` | Geçersiz veri doğrulama ayarı. |
| FileFormat | `4` | Geçersiz dosya formatı. |
| Formula | `5` | Geçersiz formül. |
| InvalidData | `6` | Geçersiz veri. |
| InvalidOperator | `7` | Geçersiz operatör. |
| IncorrectPassword | `8` | Yanlış şifre. |
| License | `9` | Lisansla ilgili hatalar. |
| Limitation | `10` | MS Excel sınırlaması dışı hata. |
| PageSetup | `11` | Geçersiz sayfa ayarı. |
| PivotTable | `12` | Geçersiz pivotTable ayarı. |
| Shape | `13` | Geçersiz çizim nesnesi ayarı. |
| Sparkline | `14` | Geçersiz sparkline nesnesi ayarı. |
| SheetName | `15` | Geçersiz çalışma sayfası adı. |
| SheetType | `16` | Geçersiz çalışma sayfası türü. |
| Interrupted | `17` | İşlem kesildi. |
| IO | `18` | Dosya geçersiz. |
| Permission | `19` | Bu dosyayı açmak için izin gerekir. |
| UnsupportedFeature | `20` | Desteklenmeyen özellik. |
| UnsupportedStream | `21` | Açılacak desteklenmeyen akış. |
| UndisclosedInformation | `22` | Dosyalar bazı açıklanmamış bilgiler içeriyor. |
| FileCorrupted | `23` | Dosya içeriği bozulmuş. |
| DefinedName | `25` | Geçersiz tanımlı ad |
| Font | `26` | Geçersiz yazı tipi |
| AutoFilter | `27` | Geçersiz otomatik filtre ayarı. |
| FontSubstitution | `28` | Yazı tipi bulunamadığında alınabilecek yazı tipi ikame uyarı türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExceptionTypeDemo
    {
        public static void ExceptionTypeExample()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();

                // Geçersiz bir çalışma sayfası adı ayarlamaya çalışarak bir istisna tetiklemek
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Çalışma kitabını kaydedin
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // CellsException'ı ele al
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // İstisna tipini kontrol edin
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Farklı istisna tipleri için gerektiği gibi daha fazla durum ekleyin
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Diğer tüm istisnaları ele alın
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


