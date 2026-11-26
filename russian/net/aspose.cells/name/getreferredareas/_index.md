---
title: "Name.GetReferredAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Name. Получает все ссылки, указанные этим именем"
type: docs
url: /ru/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Получает все ссылки, на которые ссылается это имя.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пересчитать | Boolean | нужно ли пересчитать его, если это имя уже было вычислено до этого вызова. |

### Возвращаемое значение

Все диапазоны.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            
            // Добавить некоторые данные в рабочий лист
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // Создать именованный диапазон с несколькими ссылками
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // Получить ссылочные области с внешними ссылками
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // Отобразить информацию о каждой ссылочной области
            Console.WriteLine("Number of referred areas: " + ras.Length);
            for (int i = 0; i < ras.Length; i++)
            {
                ReferredArea ra = ras[i];
                Console.WriteLine($"\nArea {i + 1}:");
                Console.WriteLine($"IsExternalLink: {ra.IsExternalLink}");
                if (ra.IsExternalLink)
                {
                    Console.WriteLine($"ExternalFileName: {ra.ExternalFileName}");
                }
                Console.WriteLine($"SheetName: {ra.SheetName}");
                Console.WriteLine($"IsArea: {ra.IsArea}");
                
                if (ra.IsArea)
                {
                    Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
                                    $" to {CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
                }
                else
                {
                    Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
                }
            }
            
            // Создать внешнюю рабочую книгу и обновить значения
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // Обновить связанный источник данных
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // Отобразить некоторые значения из ссылочных областей
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### См. также

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


