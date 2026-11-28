---
title: "Name.GetReferredAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name yöntemi. Bu ad tarafından başvurulan tüm referansları alır"
type: docs
url: /tr/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Bu ad tarafından referans verilen tüm referansları alır.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yeniden hesapla | Boolean | Bu ad bu çağrıdan önce hesaplandıysa yeniden hesaplayıp hesaplamama. |

### Dönüş Değeri

Tüm aralıklar.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Çalışma sayfasına bazı veriler ekle
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // Birden fazla referansa sahip bir adlandırılmış aralık oluştur
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // Harici bağlantılarla başvurulan alanları al
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // Her başvurulan alan hakkında bilgi göster
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
            
            // Harici bir çalışma kitabı oluştur ve değerleri güncelle
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // Bağlantılı veri kaynağını güncelle
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // Başvurulan alanlardan bazı değerleri göster
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### Ayrıca Bakınız

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


