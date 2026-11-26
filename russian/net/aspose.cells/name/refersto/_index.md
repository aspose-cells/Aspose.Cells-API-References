---
title: "Name.RefersTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Name property. Возвращает или задает формулу, к которой имя определено ссылаться, начиная со знака равенства"
type: docs
url: /ru/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Возвращает или задаёт формулу, к которой определено имя, начиная со знака равенства.

```csharp
public string RefersTo { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // Добавьте именованные диапазоны с RefersTo
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // Отобразите свойство RefersTo именованных диапазонов
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


