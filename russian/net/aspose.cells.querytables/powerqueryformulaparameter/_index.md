---
title: "Класс PowerQueryFormulaParameter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.QueryTables.PowerQueryFormulaParameter. Представляет параметр формулы Power Query."
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

Представляет параметр формулы Power Query.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Получает и задает описание формулы Power Query.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Получает определение параметра. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Получает название группы, содержащей эту формулу Power Query.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Получает и задает название формулы Power Query.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Obsolete.**) Получает определение параметра. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Получает все элементы формулы Power Query.(Inherited from [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Получает тип формулы Power Query. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Получает значение параметра. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterDemo
    {
        public static void PowerQueryFormulaParameterExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Получить доступ к свойству DataMashup рабочей книги
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Получить доступ к свойству PowerQueryFormulas
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Получить доступ к свойству PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Пример использования: перебрать PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Пример использования: перебор PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Показать детали параметра
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Сохраните книгу
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


