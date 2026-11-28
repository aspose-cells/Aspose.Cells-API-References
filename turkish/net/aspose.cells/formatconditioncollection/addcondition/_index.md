---
title: "FormatConditionCollection.AddCondition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatConditionCollection yöntemi. Bir biçimlendirme koşulu ekler"
type: docs
url: /tr/net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Bir biçimlendirme koşulu ekler.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | FormatConditionType | Biçim koşulunun türü. |
| operatorType | OperatorType | Operatör türü |
| formula1 | String | Koşullu biçimlendirme ile ilişkili değer veya ifade. Giriş değeri '=' ile başlıyorsa, formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak kabul edilir. '=' ile başlayan metin değeri için kullanıcı, formül olarak "=\"=...\"" biçiminde girebilir. |
| formula2 | String | Koşullu biçimlendirme ile ilişkili değer veya ifade. Giriş biçimi formula1 ile aynıdır. |

### Dönüş Değeri

Biçimlendirme koşulu nesne dizini;

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeOperatorTypDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;
            fcs.AddArea(ca);
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Red;
            
            conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");
            fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Green;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Bir biçim koşulu ekle.

```csharp
public int AddCondition(FormatConditionType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | FormatConditionType | Biçim koşulu türü. |

### Dönüş Değeri

Biçimlendirme koşulu nesne dizini;

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Biçim koşulları oluştur
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            
            // Aralık ekle
            CellArea area = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 5,
                EndColumn = 5
            };
            conditions.AddArea(area);

            // Koşulları ekle (int dizin döndürür)
            conditions.AddCondition(FormatConditionType.ColorScale);
            conditions.AddCondition(FormatConditionType.IconSet);
            conditions.AddCondition(FormatConditionType.DataBar);

            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


