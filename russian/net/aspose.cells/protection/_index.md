---
title: "Класс Protection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Protection. Представляет различные типы параметров защиты, доступных для листа."
type: docs
url: /ru/net/aspose.cells/protection/
---
## Protection class

Представляет различные типы параметров защиты, доступные для листа.

```csharp
public class Protection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | Представляет, разрешено ли удаление столбцов на защищённом листе. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | Представляет, разрешено ли удаление строк на защищённом листе. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | Представляет, разрешено ли пользователю манипулировать объектами рисования на защищённом листе. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | Представляет, разрешено ли пользователю использовать автофильтр, созданный до защиты листа. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | Представляет, разрешено ли форматирование ячеек на защищённом листе. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | Представляет, разрешено ли форматирование столбцов на защищённом листе |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | Представляет, разрешено ли форматирование строк на защищённом листе |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | Представляет, разрешено ли вставка столбцов на защищённом листе |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | Представляет, разрешено ли вставка гиперссылок на защищённом листе |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | Представляет, разрешено ли вставка строк на защищённом листе |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | Представляет, разрешена ли опция сортировки на защищённом листе. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | Представляет, разрешено ли пользователю манипулировать сводными таблицами на защищённом листе. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | Указывает, защищён ли лист паролем. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | Представляет пароль для защиты листа. |

## Методы

| Имя | Описание |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | Копировать информацию о защите. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | Получает хеш текущего пароля. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | Проверяет пароль. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionDemo
    {
        public static void ProtectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к настройкам защиты листа
            Protection protection = worksheet.Protection;

            // Установка различных свойств защиты
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Проверка, защищён ли лист паролем
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Сохранение книги
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


