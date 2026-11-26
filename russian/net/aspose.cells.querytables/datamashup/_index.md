---
title: "Класс DataMashup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.QueryTables.DataMashup. Представляет данные mashup"
type: docs
url: /ru/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

Представляет данные mashup.

```csharp
public class DataMashup
```

## Свойства

| Имя | Описание |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Устарело.**) Получает параметры формулы Power Query. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Получает все формулы Power Query. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class DataMashupDemo
    {
        public static void DataMashupExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к свойству DataMashup рабочей книги
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // Получить доступ к свойству PowerQueryFormulas
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Получить доступ к свойству PowerQueryFormulaParameters
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Пример использования: перебрать PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Пример использования: перебор PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Сохраните книгу
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


