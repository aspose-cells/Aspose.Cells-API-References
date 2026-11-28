---
title: "SpreadsheetLocker.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpreadsheetLocker yöntemi. Belirtilen ayarlarla elektronik tablo dosyasını kilitler"
type: docs
url: /tr/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFile | String | Kilitlemek için şablon dosyası |
| resultFile | String | Ortaya çıkan dosya |
| openPassword | String | Dosya şifrelemesi için parola |
| writePassword | String | Elektronik tabloyu değiştirme koruması için parola |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
    {
        public static void Run()
        {           
            string templatePath = "template.xlsx";            
            // Sonuç dosya yolunu hazırla
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Tipi kullanarak string parametrelerle Process yöntemini doğrudan çalıştır
                SpreadsheetLocker.Process(
                    templateFile: templatePath,
                    resultFile: resultPath,
                    openPassword: "Open@123",
                    writePassword: "Write@456"
                );

                Console.WriteLine($"Spreadsheet secured successfully. Saved to: {Path.GetFullPath(resultPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error securing spreadsheet: {ex.Message}");
            }
            finally
            {
                // Geçici şablonu temizle
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Giriş ve yükleme seçenekleri |
| saveOptions | LowCodeSaveOptions | Çıktı ve kaydetme seçenekleri |
| openPassword | String | Dosya şifrelemesi için parola |
| writePassword | String | Elektronik tabloyu değiştirme koruması için parola |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            
            // Tabloyu kilitleme/açma şifreleriyle işleyin
            SpreadsheetLocker.Process(
                new LowCodeLoadOptions() { InputFile = "input.xlsx" },
                new LowCodeSaveOptions() 
                { 
                    OutputFile = "output_locked.xlsx" 
                }, 
                "123456", 
                "234567");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Giriş ve yükleme seçenekleri |
| saveOptions | LowCodeSaveOptions | Çıktı ve kaydetme seçenekleri |
| openPassword | String | Dosya şifrelemesi için parola |
| writePassword | String | Elektronik tabloyu değiştirme koruması için parola |
| workbookPassword | String | Çalışma kitabının korunması için şifre |
| workbookType | ProtectionType | Çalışma kitabını korumak için koruma türü |

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Belirtilen ayarlarla elektronik tablo dosyasını kilitler.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Giriş ve yükleme seçenekleri |
| saveOptions | LowCodeSaveOptions | Çıktı ve kaydetme seçenekleri |
| sağlayıcı | AbstractLowCodeProtectionProvider | Koruma ayarlarını sağlamak için uygulama |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
           
            // LowCodeLoadOptions'ı hazırlayın
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // LowCodeSaveOptions'ı hazırlayın
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Özel bir koruma sağlayıcı oluşturun
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Belirtilen parametrelerle statik Process metodunu çağırın
                SpreadsheetLocker.Process(loadOptions, saveOptions, provider);

                Console.WriteLine("Spreadsheet processed and protected successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error processing spreadsheet: {ex.Message}");
            }

        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override string GetOpenPassword()
            {
                return "open123";
            }

            public override string GetWritePassword()
            {
                return "write123";
            }

            public override string GetWorkbookPassword()
            {
                return "workbook123";
            }

            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.All;
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


