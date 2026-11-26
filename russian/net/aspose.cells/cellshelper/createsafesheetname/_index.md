---
title: "CellsHelper.CreateSafeSheetName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Проверяет заданное имя листа и при необходимости создает корректное. Если заданное имя листа соответствует правилам имен листов Excel, то возвращает его. В противном случае строка будет обрезана, если длина превышает ограничение, а недопустимые символы будут заменены   затем возвращается восстановленное строковое значение."
type: docs
url: /ru/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены на ' ', затем возвращается восстановленное значение строки.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| nameProposal | String | имя листа, которое будет использоваться |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Проверяет указанное имя листа и при необходимости создает корректное. Если указанное имя листа соответствует правилам имен листов Excel, возвращает его. В противном случае строка будет усечена, если её длина превышает ограничение, а недопустимые символы будут заменены заданным символом, затем возвращается восстановленное значение строки.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| nameProposal | String | имя листа, которое будет использоваться |
| replaceChar | Char | символ, который будет использоваться для замены недопустимых символов в указанном имени листа |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // Пример 1: Создать безопасное имя листа с символом замены по умолчанию
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // Пример 2: Создать безопасное имя листа с пользовательским символом замены 'A'
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


