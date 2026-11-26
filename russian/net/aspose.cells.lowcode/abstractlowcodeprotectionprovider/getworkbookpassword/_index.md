---
title: "AbstractLowCodeProtectionProvider.GetWorkbookPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeProtectionProvider. Получает пароль для защиты книги с указанным типом защиты"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/
---
## AbstractLowCodeProtectionProvider.GetWorkbookPassword method

Получает пароль для защиты книги с указанным типом защиты.

```csharp
public virtual string GetWorkbookPassword()
```

### Возвращаемое значение

Пароль для защиты книги.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorkbookPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var provider = new DemoProtectionProvider();

            try
            {
                string password = provider.GetWorkbookPassword();
                ProtectionType protectionType = provider.GetWorkbookProtectionType();

                workbook.Protect(protectionType, password);
                Console.WriteLine($"Workbook protected with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ProtectedWorkbook.xlsx");

        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWorkbookPassword()
        {
            return "Aspose1234!";
        }

        public override ProtectionType GetWorkbookProtectionType()
        {
            return ProtectionType.Structure;
        }
        
    }
}
```

### См. также

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


