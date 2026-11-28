---
title: "Worksheet.Replace"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Tüm hücre metinlerini yeni bir dizeyle değiştirir"
type: docs
url: /tr/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Tüm hücrelerin metnini yeni bir dizeyle değiştirir.

```csharp
public int Replace(string oldString, string newString)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldString | String | Eski dize değeri. |
| newString | String | Yeni dize değeri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // Örnek metinle bir metin kutusu ekle
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // Üstbilgi ve altbilgiyi ayarla
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // Tüm içerikte "Hello" yerine "Hi" değiştir
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // Üstbilgi/altbilgilerde değiştir
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // Metin kutularında değiştir
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


