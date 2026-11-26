---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataMashup. Возвращает параметры формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Возвращает параметры формулы Power Query.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство DataMashup.PowerQueryFormulas. Это свойство будет удалено через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulaParametersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к свойству DataMashup
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Получить доступ к PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // Отобразить количество параметров
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // Итерировать параметры, если они существуют
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // Сохраните книгу
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


