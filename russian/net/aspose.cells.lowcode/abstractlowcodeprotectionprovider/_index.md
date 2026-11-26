---
title: "Класс AbstractLowCodeProtectionProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LowCode.AbstractLowCodeProtectionProvider класс. Реализация для предоставления параметров защиты"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/
---
## AbstractLowCodeProtectionProvider class

Реализация, предоставляющая настройки защиты

```csharp
public class AbstractLowCodeProtectionProvider
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AbstractLowCodeProtectionProvider](abstractlowcodeprotectionprovider/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [GetOpenPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/)() | Получает пароль для открытия файла электронной таблицы. |
| virtual [GetWorkbookPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/)() | Получает пароль для защиты книги с указанным типом защиты. |
| virtual [GetWorkbookProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/)() | Получает тип защиты для защиты книги. |
| virtual [GetWorksheetPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/)(string) | Получает пароль для защиты указанного листа. |
| virtual [GetWorksheetProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/)(string) | Получает тип защиты для защиты указанного листа. |
| virtual [GetWritePassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/)() | Получает пароль для изменения файла электронной таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeProtectionProviderDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и добавьте тестовые листы
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("AuditReport");

            // Создайте экземпляр пользовательского провайдера защиты
            var protectionProvider = new CustomProtectionProvider();

            // Примените защиту книги
            workbook.Protect(
                protectionProvider.GetWorkbookProtectionType(),
                protectionProvider.GetWorkbookPassword()
            );

            // Примените защиту ко всем листам
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                worksheet.Protect(
                    protectionProvider.GetWorksheetProtectionType(worksheet.Name),
                    null,  // Add null for oldPassword parameter
                    protectionProvider.GetWorksheetPassword(worksheet.Name)
                );
            }

            // Установите пароли доступа к файлу
            workbook.Settings.Password = protectionProvider.GetOpenPassword();
            workbook.Settings.WriteProtection.Password = protectionProvider.GetWritePassword();

            // Сохраните защищённую книгу
            workbook.Save("AbstractLowCodeProtectionProviderDemo.xlsx");
        }
    }

    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword() => "SecureOpen123";
        public override string GetWritePassword() => "EditPermission456";
        public override string GetWorkbookPassword() => "WorkbookLock789";
        
        public override ProtectionType GetWorkbookProtectionType() => 
            ProtectionType.Windows;  // Prevent window structure changes

        public override string GetWorksheetPassword(string sheetName) => 
            $"SheetLock_{sheetName}";  // Dynamic password per sheet

        public override ProtectionType GetWorksheetProtectionType(string sheetName) => 
            ProtectionType.Contents;  // Protect cell contents
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


