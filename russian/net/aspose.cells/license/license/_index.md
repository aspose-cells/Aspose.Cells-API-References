---
title: "License.License"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор License. Инициализирует новый экземпляр этого класса"
type: docs
url: /ru/net/aspose.cells/license/license/
---
## License constructor

Инициализирует новый экземпляр этого класса.

```csharp
public License()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте новый экземпляр License, используя конструктор (#ctor)
            License license = new License();
            
            // Установите файл лицензии
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### См. также

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


