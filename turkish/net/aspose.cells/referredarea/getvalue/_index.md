---
title: "ReferredArea.GetValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReferredArea yöntemi. Bu alanın sol üst köşesinden verilen offset ile hücre değerini alır"
type: docs
url: /tr/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Bu alanın sol üst köşesinden verilen offset ile hücre değerini alır.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | Int32 | Bu alanın başlangıç satırından satır offset'i |
| colOffset | Int32 | Bu alanın başlangıç satırından sütun offset'i |

### Dönüş Değeri

"#REF!" bu alan geçersizse; "#N/A" verilen offset bu alanın dışındaysa; Aksi takdirde belirtilen konumdaki hücre değerini döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = "=A1";
            
            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                object value = referredAreas[0].GetValue(0, 0);
                Console.WriteLine("Value at (0,0): " + value);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Bu alanın sol üst köşesinden verilen offset ile hücre değerini alır.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | Int32 | Bu alanın başlangıç satırından satır offset'i |
| colOffset | Int32 | Bu alanın başlangıç satırından sütun offset'i |
| calculateFormulas | Boolean | Belirtilen referans bir formül ise yinelemeli olarak hesaplanıp hesaplanmayacağı |

### Dönüş Değeri

"#REF!" bu alan geçersizse; "#N/A" verilen offset bu alanın dışındaysa; Aksi takdirde belirtilen konumdaki hücre değerini döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(100);
            sheet.Cells["B1"].PutValue(200);

            workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names["TestRange"];
            name.RefersTo = "=Sheet1!$A$1:$B$1";

            ReferredArea ra = name.GetReferredAreas(true)[0];
            object result = ra.GetValue(0, 0, true);

            Console.WriteLine("Obtained value: " + result);
        }
    }
}
```

### Ayrıca Bakınız

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


