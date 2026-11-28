---
title: "TxtLoadOptions.ExtendToNextSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Veri satırları veya sütunları limit aşınca veriyi bir sonraki sayfaya genişletip genişletmeyeceği. Varsayılan false'tur"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Veri satırları veya sütunları sınırı aştığında veriyi bir sonraki sayfaya genişletip genişletmeyeceği. Varsayılan değer false'tur.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Açıklamalar

Bu özellik true ise, ekstra veri mevcut sayfanın arkasındaki bir sonraki sayfaya konulacaktır (eğer mevcut sayfa son sayfa ise, yeni sayfa mevcut çalışma kitabına eklenecektir). Bu özellik false ise, limit aşan veri yok sayılacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyExtendToNextSheetDemo
    {
        public static void Run()
        {
            // Normal çalışma sayfası sütun limitlerini aşan örnek bir CSV dizesi oluşturun
            string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";

            // ExtendToNextSheet etkinleştirilmiş TxtLoadOptions oluşturun
            TxtLoadOptions options = new TxtLoadOptions
            {
                ExtendToNextSheet = true
            };

            // CSV verisinden bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);

            // İlk çalışma sayfasındaki hücreleri alın
            Cells cells = workbook.Worksheets[0].Cells;

            // İçe aktarılan veri hakkında bilgi çıktısı verin
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

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


