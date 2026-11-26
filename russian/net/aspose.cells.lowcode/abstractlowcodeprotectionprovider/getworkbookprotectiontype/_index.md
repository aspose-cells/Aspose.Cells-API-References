---
title: "AbstractLowCodeProtectionProvider.GetWorkbookProtectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeProtectionProvider. Получает тип защиты для защиты книги"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorkbookProtectionType method

Получает тип защиты для защиты книги.

```csharp
public virtual ProtectionType GetWorkbookProtectionType()
```

### Возвращаемое значение

Тип защиты для защиты книги. None означает отсутствие защиты для книги.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorkbookProtectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            var provider = new CustomProtectionProvider();

            try
            {
                workbook.Protect(provider.GetWorkbookProtectionType(), provider.GetWorkbookPassword());
                
                ProtectionType protectionType = provider.GetWorkbookProtectionType();
                Console.WriteLine($"Workbook protection type: {protectionType}");
                Console.WriteLine($"Protection status: {workbook.Settings.IsProtected}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorkbookProtectionType: {ex.Message}");
            }

            workbook.Save("WorkbookProtectionDemo.xlsx");
        }


        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.Structure;
            }

            public override string GetWorkbookPassword()
            {
                return "aspose123";
            }
        }
    }
}
```

### См. также

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


