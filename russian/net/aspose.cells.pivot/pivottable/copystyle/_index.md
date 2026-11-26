---
title: "PivotTable.CopyStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Копирует именованный стиль из другой сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Копирует именованный стиль из другой сводной таблицы.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | PivotTable | Исходная сводная таблица. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // Создать исходную книгу с сводной таблицей
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Добавьте примерные данные
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // Создать исходную сводную таблицу (явно получить объект сводной таблицы)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Применить стиль к исходной сводной таблице
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Создать целевую книгу с сводной таблицей
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Добавить ту же структуру данных
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // Создать целевую сводную таблицу (явно получить объект сводной таблицы)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Скопировать стиль из исходной в целевую сводную таблицу
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // Сохранить результат
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


