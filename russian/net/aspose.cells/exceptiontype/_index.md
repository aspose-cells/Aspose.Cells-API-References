---
title: "Перечисление ExceptionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExceptionType. Представляет код пользовательского типа исключения"
type: docs
url: /ru/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Представляет код пользовательского типа исключения.

```csharp
public enum ExceptionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Chart | `0` | Недопустимая настройка диаграммы. |
| DataType | `1` | Недопустимая настройка типа данных. |
| DataValidation | `2` | Недопустимая настройка проверки данных. |
| ConditionalFormatting | `3` | Недопустимая настройка проверки данных. |
| FileFormat | `4` | Недопустимый формат файла. |
| Formula | `5` | Недопустимая формула. |
| InvalidData | `6` | Недопустимые данные. |
| InvalidOperator | `7` | Недопустимый оператор. |
| IncorrectPassword | `8` | Неправильный пароль. |
| License | `9` | Ошибки, связанные с лицензией. |
| Limitation | `10` | Ошибка превышения ограничений MS Excel. |
| PageSetup | `11` | Недопустимая настройка разметки страницы. |
| PivotTable | `12` | Недопустимая настройка сводной таблицы. |
| Shape | `13` | Недопустимая настройка графического объекта. |
| Sparkline | `14` | Недопустимая настройка объекта спарклайна. |
| SheetName | `15` | Недопустимое имя листа. |
| SheetType | `16` | Недопустимый тип листа. |
| Interrupted | `17` | Процесс прерван. |
| IO | `18` | Файл недействителен. |
| Permission | `19` | Для открытия этого файла требуется разрешение. |
| UnsupportedFeature | `20` | Функция не поддерживается. |
| UnsupportedStream | `21` | Открытие неподдерживаемого потока. |
| UndisclosedInformation | `22` | Файлы содержат некоторую неразглашённую информацию. |
| FileCorrupted | `23` | Содержимое файла повреждено. |
| DefinedName | `25` | Недопустимое определённое имя |
| Font | `26` | Недопустимый шрифт |
| AutoFilter | `27` | Недопустимая настройка автофильтра. |
| FontSubstitution | `28` | Тип предупреждения о замене шрифта, когда шрифт не найден; этот тип предупреждения может быть получен. |

### Примеры

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
                // Создать новую книгу
                Workbook workbook = new Workbook();

                // Попытка установить недопустимое имя листа, чтобы вызвать исключение
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Сохраните книгу
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // Обработать CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // Проверьте тип исключения
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Добавьте дополнительные случаи по мере необходимости для разных типов исключений
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Обработайте любые другие исключения
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


