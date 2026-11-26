---
title: "Класс CopyOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CopyOptions. Представляет параметры копирования"
type: docs
url: /ru/net/aspose.cells/copyoptions/
---
## CopyOptions class

Представляет параметры копирования.

```csharp
public class CopyOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CopyOptions](copyoptions/)() | Конструктор CopyOptions. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Указывает, копировать ли ширину столбца в единицах символов. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | Если формула недействительна для целевого назначения, копировать только значения. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | Указывает, копировать ли имена. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Указывает, расширять ли диапазоны при копировании диапазона в соседний диапазон. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Указывает, сохранять ли макросы; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | При копировании диапазона в том же файле, если диаграмма ссылается на исходный лист, значение False означает, что источник данных скопированной диаграммы не будет изменён. Значение True означает, что источник данных скопированной диаграммы будет ссылаться на лист назначения. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | В MS Excel при копировании формул, которые ссылаются на другие листы, при копировании листа в другой, скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы уже были скопированы до этой операции копирования; в этом случае свойство следует оставить истинным. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | Указывает, ссылаться ли на целевой лист, если указанный лист не был скопирован. |

### Примеры

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Создать новую книгу для копирования данных
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Создать объект CopyOptions
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Скопировать данные из исходного листа в целевой лист
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Сохранить целевую книгу
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


