---
title: "FormatConditionCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FormatConditionCollection. Добавляет условие форматирования и затронутый диапазон ячеек в FormatConditions. FormatConditions могут содержать до трёх условных форматов. Ссылки на другие листы не допускаются в формулах условного форматирования"
type: docs
url: /ru/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Добавляет условие форматирования и затронутый диапазон ячеек в FormatConditions. FormatConditions может содержать до трёх условных форматов. Ссылки на другие листы не допускаются в формулах условного форматирования.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | Диапазон ячеек с условным форматированием. |
| type | FormatConditionType | Тип условного форматирования. Это может быть один из членов FormatConditionType. |
| operatorType | OperatorType | Оператор сравнения. Это может быть один из членов OperatorType. |
| formula1 | String | Значение или выражение, связанное с условным форматированием. |
| formula2 | String | Значение или выражение, связанное с условным форматированием |

### Возвращаемое значение

[0]:Formatting condition object index;[1] Effected cell rang index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Заполнить примерными данными
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Добавить условное форматирование
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // Продемонстрировать метод Add с указанными параметрами
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // Применить форматирование
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // Сохранить книгу, чтобы продемонстрировать результат
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


