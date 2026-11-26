---
title: "PdfSecurityOptions.UserPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSecurityOptions. Получает или задает пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа"
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Получает или задаёт пользовательский пароль, необходимый для открытия зашифрованного PDF‑документа.

```csharp
public string UserPassword { get; set; }
```

### Примечания

Для просмотра зашифрованного PDF‑документа потребуется пароль владельца или пользовательский пароль.

Пользовательский пароль может быть null или пустой строкой; в этом случае при открытии PDF‑документа пароль от пользователя не требуется.

Открытие документа с правильным паролем владельца предоставляет полный доступ к документу.

Открытие документа с правильным пользовательским паролем (или открытие документа без пользовательского пароля) предоставляет ограниченный доступ в соответствии с указанными разрешениями.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyUserPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with User Password";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            
            securityOptions.UserPassword = "user123";
            securityOptions.OwnerPassword = "owner456";
            securityOptions.PrintPermission = true;
            
            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("ProtectedWithUserPassword.pdf", saveOptions);
            
            Console.WriteLine("PDF created with user password protection.");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


