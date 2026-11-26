---
title: "Класс License"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.License. Предоставляет методы для лицензирования компонента"
type: docs
url: /ru/net/aspose.cells/license/
---
## License class

Предоставляет методы лицензирования компонента.

```csharp
public class License
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [License](license/)() | Инициализирует новый экземпляр этого класса. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Лицензирует компонент. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Лицензирует компонент. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // Создайте экземпляр класса License
            License license = new License();

            // Установите лицензию, используя имя файла лицензии
            license.SetLicense("Aspose.Cells.NET.lic");

            // В качестве альтернативы установите лицензию, используя поток
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // Дополнительный код, демонстрирующий использование лицензированной функциональности Aspose.Cells
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // Сохраните книгу, чтобы проверить, что лицензия применена корректно
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


