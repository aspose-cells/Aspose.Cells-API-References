---
title: "FindOptions.RegexKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Указывает, является ли искомый ключ регулярным выражением. Если true, ключ будет восприниматься как регулярное выражение и разбираться. В противном случае ключ будет обрабатываться согласно правилам MS Excel."
type: docs
url: /ru/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Указывает, является ли искомый ключ регулярным выражением. Если true, искомый ключ будет восприниматься как регулярное выражение и анализироваться. В противном случае ключ будет анализироваться согласно правилам в MS Excel.

```csharp
public bool RegexKey { get; set; }
```

### Примечания

Несмотря на то, что ключ поиска указан как регулярное выражение, он может быть преобразован в соответствии с указанным [`LookAtType`](../lookattype/). Например, когда тип установлен в Contains (это значение по умолчанию для этих параметров), подстановочные знаки будут автоматически добавлены в начало и конец ключа поиска, чтобы обеспечить проверку совпадения как "contains". В этом случае регулярные выражения станут более сложными, и производительность также снизится. Поэтому, учитывая производительность, если пользователь указал точное правило для регулярного выражения, нет необходимости использовать [`LookAtType`](../lookattype/) как дополнительное ограничение, и пользователь может установить его в EntireContent для получения лучшей производительности.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите тестовые данные со строками, соответствующими шаблону
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // Создайте параметры поиска с включённым regex
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // Ищите ячейки, соответствующие шаблону regex
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // Вывести результат.
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


