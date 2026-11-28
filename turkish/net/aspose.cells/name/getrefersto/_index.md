---
title: "Name.GetRefersTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name yöntemi. Bu Name'in referansını alın"
type: docs
url: /tr/net/aspose.cells/name/getrefersto/
---
## GetRefersTo(bool, bool) {#getrefersto}

Bu Name'in referansını al.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | Boolean | Referansın R1C1 olarak biçimlendirilip biçimlendirilmediği. |
| isLocal | Boolean | Referansın yerel ayara göre biçimlendirilip biçimlendirilmediği. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // GetRefersTo'yi R1C1 formatı ve yerel kapsam ile çağırın
                string refersToR1C1Local = namedRange.GetRefersTo(true, true);
                Console.WriteLine("R1C1 format with local scope: " + refersToR1C1Local);

                // GetRefersTo'yi A1 formatı ve küresel kapsam ile çağırın
                string refersToA1Global = namedRange.GetRefersTo(false, false);
                Console.WriteLine("A1 format with global scope: " + refersToA1Global);

                // Adlandırılmış aralık ayrıntılarını göster
                Console.WriteLine("Named range text: " + namedRange.Text);
                Console.WriteLine("Full text: " + namedRange.FullText);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("NameMethodGetRefersToDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRefersTo(bool, bool, int, int) {#getrefersto_1}

Belirtilen hücreye göre bu Name'in referansını al.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal, int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | Boolean | Referansın R1C1 olarak biçimlendirilip biçimlendirilmediği. |
| isLocal | Boolean | Referansın yerel ayara göre biçimlendirilip biçimlendirilmediği. |
| satır | Int32 | Hücrenin satır indeksi. |
| sütun | Int32 | Hücrenin sütun indeksi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // GetRefersTo'yi belirli parametrelerle (isR1C1, isLocal, row, column) çağırın
                string refersTo = namedRange.GetRefersTo(false, false, 0, 0);
                
                Console.WriteLine("Named range refers to: " + refersTo);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");

                // Sonuca göre adlandırılmış aralığı değiştir
                if (!string.IsNullOrEmpty(refersTo))
                {
                    worksheet.Cells["B1"].PutValue("Named Range Refers To:");
                    worksheet.Cells["B2"].PutValue(refersTo);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


