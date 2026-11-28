---
title: "WorkbookSettings.IsEncrypted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Bu çalışma kitabını açmak için bir parolanın gerekli olup olmadığını gösteren bir değer alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/isencrypted/
---
## WorkbookSettings.IsEncrypted property

Bu çalışma kitabını açmak için bir şifre gerekip gerekmediğini gösteren bir değeri alır.

```csharp
public bool IsEncrypted { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Örnek 1: Parola korumalı bir çalışma kitabının şifrelenip şifrelenmediğini kontrol et
            string encryptedFilePath = "encrypted.xlsx";
            var encryptedWorkbook = new Workbook(encryptedFilePath, new LoadOptions { Password = "password" });
            Console.WriteLine($"Encrypted workbook IsEncrypted: {encryptedWorkbook.Settings.IsEncrypted}");

            // Örnek 2: Normal bir çalışma kitabının şifrelenip şifrelenmediğini kontrol et
            string normalFilePath = "normal.xlsx";
            var normalWorkbook = new Workbook(normalFilePath);
            Console.WriteLine($"Normal workbook IsEncrypted: {normalWorkbook.Settings.IsEncrypted}");

            // Örnek 3: Şifreli bir çalışma kitabı oluştur ve kaydet
            var newWorkbook = new Workbook();
            newWorkbook.Settings.Password = "12345";
            newWorkbook.Save("new_encrypted.xlsx");
            Console.WriteLine($"New workbook IsEncrypted: {newWorkbook.Settings.IsEncrypted}");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


