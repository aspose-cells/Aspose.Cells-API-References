---
title: "SheetSet.SheetSet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetSet yapıcı. Belirli sayfa indekslerine göre bir sayfa kümesi oluşturur"
type: docs
url: /tr/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

Tam sayfa indekslerine göre bir sayfa seti oluşturur.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndexes | Int32[] | sıfır tabanlı sayfa indeksleri. |

### Açıklamalar

Çalışma kitabında bulunmayan bir sayfa ile karşılaşıldığında, işleme sırasında bir istisna fırlatılacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // 3 çalışma sayfası içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Her sayfaya tanımlama metni ekleyin
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // Belirli sayfa indeksleri (0 ve 2) ile SheetSet oluşturun
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // Sayfa kümemizle PDF kaydetme seçenekleri oluşturun
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // Seçili sayfalarla çalışma kitabını kaydedin
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

Tam sayfa adlarına göre bir sayfa seti oluşturur.

```csharp
public SheetSet(params string[] sheetNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetNames | String[] | sayfa adları. |

### Açıklamalar

Çalışma kitabında bulunmayan bir sayfa ile karşılaşıldığında, işleme sırasında bir istisna fırlatılacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve sayfalar ekleyin
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // SheetSet için sayfa adlarını hazırlayın
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // Dize dizisi parametresiyle SheetSet oluşturun
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // Oluşturulan SheetSet ile PDF kaydetme seçeneklerini yapılandırın
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // Belirtilen sayfalarla çalışma kitabını PDF olarak kaydedin
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


