---
title: "Класс Validation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Validation. Представляет настройки проверки данных"
type: docs
url: /ru/net/aspose.cells/validation/
---
## Validation class

Представляет настройки проверки данных.

```csharp
public class Validation
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | Представляет стиль оповещения проверки. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | Получает все [`CellArea`](../cellarea/), содержащие настройки проверки данных. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | Представляет сообщение об ошибке проверки данных. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | Представляет заголовок диалогового окна ошибки проверки данных. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | Представляет значение или выражение, связанное с проверкой данных. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | Представляет значение или выражение, связанное с проверкой данных. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | Указывает, разрешены ли пустые значения в проверке диапазона данных. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | Указывает, отображает ли проверка данных выпадающий список с допустимыми значениями. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | Представляет вводное сообщение проверки данных. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | Представляет заголовок диалогового окна ввода проверки данных. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | Представляет оператор для проверки данных. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | Указывает, будет ли вводное сообщение проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | Представляет тип проверки данных. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | Представляет первое значение, связанное с проверкой данных. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | Представляет второе значение, связанное с проверкой данных. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | Применяет проверку к области. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | Применяет проверку к области. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | Применяет проверку к указанным областям. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | Копировать проверку. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | Получает значение или выражение, связанное с этой проверкой. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | Получает значение или выражение, связанное с этой проверкой. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | Получает значение или выражение, связанное с этой проверкой для конкретной ячейки. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | Получить значение списка проверок для указанной ячейки. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | Получить значение проверки в конкретной ячейке. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | Удалить настройки проверки в ячейке. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | Удалить настройки проверки в диапазоне. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | Удаляет эту проверку из указанных областей. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | Устанавливает значение или выражение, связанное с этой проверкой. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | Устанавливает значение или выражение, связанное с этой проверкой. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationDemo
    {
        public static void ValidationExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Определить область ячеек для проверки
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Получить доступ к коллекции проверок
            ValidationCollection validations = worksheet.Validations;

            // Добавить новую проверку в коллекцию
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Установить свойства проверки
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;

            // Сохраните книгу
            workbook.Save("ValidationExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


