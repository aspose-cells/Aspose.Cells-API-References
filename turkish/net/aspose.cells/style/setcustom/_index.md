---
title: "Style.SetCustom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Bir hücrenin Özel sayı biçim dizesini ayarlar"
type: docs
url: /tr/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Bir hücrenin Özel sayı biçim dizesini ayarlar.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| özel | String | Özel sayı biçim dizesi, InvariantCulture desenine uygun olmalıdır. |
| builtinPreference | Boolean | Verilen Özel sayı biçim dizesi, geçerli bölgesel ayarlarla eşleşen yerleşik sayı biçimlerinden biriyle aynıysa, sayı biçimini Özel yerine yerleşik olarak ayarlayıp ayarlamama. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodSetCustomWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            
            string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat1, true);
            Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);

            string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat2, true);
            Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);

            string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
            style.SetCustom(customFormat3, true);
            Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


