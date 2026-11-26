---
title: "Класс Validation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.Validation класс."
type: docs
url: /ru/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Validation](validation/#constructor)() | Конструктор по умолчанию. |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## Свойства

| Имя | Описание |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | Получает относительную ячейку объекта.(Наследовано от [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | Получает или задает имя JavaScript функции клиентской проверки. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | Получает или задает тип операции проверки, Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | Получает или задает целевое значение оператора 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | Получает или задает целевое значение оператора 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | Получает или задает, требуется ли значение ячейки. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | Получает или задает строку регулярного выражения. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | Получает объект списка значений. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | Используется только во время проектирования. |

## Методы

| Имя | Описание |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | Загружает список значений из объекта DataView. Вы можете указать поле значения и поле текста объекта DataView. Каждая пара значения и текста будет объединена в одну строку, разделённую запятой. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. пожалуйста, используйте вместо него GridValidation. Этот класс будет удалён через 6 месяцев после августа 2014 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


