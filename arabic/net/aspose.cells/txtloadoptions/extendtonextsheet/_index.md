---
title: "TxtLoadOptions.ExtendToNextSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما يتجاوز عدد الصفوف أو الأعمدة الحد. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

ما إذا كان يمد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد. القيمة الافتراضية هي false.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### ملاحظات

إذا كانت هذه الخاصية true، سيتم وضع البيانات الإضافية في الورقة التالية خلف الحالية (إذا كانت الورقة الحالية هي الأخيرة، ستُضاف ورقة جديدة إلى دفتر العمل الحالي). إذا كانت هذه الخاصية false، سيتم تجاهل البيانات التي تتجاوز الحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyExtendToNextSheetDemo
    {
        public static void Run()
        {
            // أنشئ سلسلة CSV نموذجية تتجاوز حدود أعمدة ورقة العمل العادية
            string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";

            // أنشئ TxtLoadOptions مع تمكين ExtendToNextSheet
            TxtLoadOptions options = new TxtLoadOptions
            {
                ExtendToNextSheet = true
            };

            // أنشئ دفتر عمل من بيانات CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);

            // احصل على الخلايا من ورقة العمل الأولى
            Cells cells = workbook.Worksheets[0].Cells;

            // أخرج معلومات حول البيانات المستوردة
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

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


