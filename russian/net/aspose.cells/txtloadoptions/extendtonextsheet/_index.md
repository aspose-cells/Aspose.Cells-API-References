---
title: "TxtLoadOptions.ExtendToNextSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Указывает, расширять ли данные на следующий лист, когда количество строк или столбцов превышает лимит. По умолчанию false"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Определяет, расширять ли данные на следующий лист, когда строки или столбцы данных превышают предел. По умолчанию false.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Примечания

Если это свойство равно true, лишние данные будут помещены на следующий лист позади текущего (если текущий лист последний, будет добавлен новый лист в текущую книгу). Если это свойство равно false, данные, превышающие лимит, будут игнорироваться.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyExtendToNextSheetDemo
    {
        public static void Run()
        {
            // Создайте пример строки CSV, превышающей обычные ограничения столбцов листа
            string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";

            // Создайте TxtLoadOptions с включённым ExtendToNextSheet
            TxtLoadOptions options = new TxtLoadOptions
            {
                ExtendToNextSheet = true
            };

            // Создайте книгу из данных CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);

            // Получите ячейки с первого листа
            Cells cells = workbook.Worksheets[0].Cells;

            // Выведите информацию о импортированных данных
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
            Console.WriteLine("Columns in first worksheet: " + workbook.Worksheets[0].Cells.MaxColumn);
            
            if (workbook.Worksheets.Count > 1)
            {
                Console.WriteLine("Columns in second worksheet: " + workbook.Worksheets[1].Cells.MaxColumn);
                Console.WriteLine("First cell in second worksheet: " + workbook.Worksheets[1].Cells[0, 0].StringValue);
            }
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


