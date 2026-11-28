---
title: "ReferredArea Sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ReferredArea sınıfı. Formül tarafından başvurulan bir alanı temsil eder"
type: docs
url: /tr/net/aspose.cells/referredarea/
---
## ReferredArea class

Formül tarafından başvurulan bir alanı temsil eder.

```csharp
public class ReferredArea
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | Alanının son sütunu. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | Alanının son satırı. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Bu bir dış referans ise dış dosya adını al. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Bunun bir alan olup olmadığını gösterir. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Bu alanın tüm satırları (tam sütun) içerip içermediğini gösterir. |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Bu alanın tüm sütunları (tam satır) içerip içermediğini gösterir. |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Bunun harici bir bağlantı olup olmadığını gösterir. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Bu referansın hangi sayfada olduğunu gösterir. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Bu örneğin başvurduğu tüm çalışma sayfalarının adları. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | Alanının başlangıç sütunu. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | Alanının başlangıç satırı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Bu alanın sol üst köşesinden verilen offset ile hücre değerini alır. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Bu alanın sol üst köşesinden verilen offset ile hücre değerini alır. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Bu alandaki hücre değerlerini alır. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Bu alandaki hücre değerlerini alır. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Bu alanın referans adresini döndürür. Genel olarak, formülde kullanılabilecek referansın adresidir, örneğin "Sheet1!A1:C3". |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir aralığa başvuran bazı veriler ve bir formül ayarlayın
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // A1:B2 aralığına başvuran bir formül oluşturun
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Formülden başvurulan alanları alın
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // İlk başvurulan alanı alın
                    ReferredArea referredArea = referredAreas[0];

                    // Başvurulan alanın temel özelliklerini gösterin
                    Console.WriteLine($"Referred Area Details:");
                    Console.WriteLine($"- Is External Link: {referredArea.IsExternalLink}");
                    Console.WriteLine($"- Sheet Name: {referredArea.SheetName}");
                    Console.WriteLine($"- Start Row: {referredArea.StartRow}");
                    Console.WriteLine($"- Start Column: {referredArea.StartColumn}");
                    Console.WriteLine($"- End Row: {referredArea.EndRow}");
                    Console.WriteLine($"- End Column: {referredArea.EndColumn}");
                    Console.WriteLine($"- Is Area: {referredArea.IsArea}");
                    Console.WriteLine($"- Is Entire Row: {referredArea.IsEntireRow}");
                    Console.WriteLine($"- Is Entire Column: {referredArea.IsEntireColumn}");

                    // Başvurulan alandan değerleri alın
                    object values = referredArea.GetValues();
                    if (values is Array)
                    {
                        object[][] valueArray = (object[][])values;
                        Console.WriteLine("\nValues in the referred area:");
                        foreach (object[] row in valueArray)
                        {
                            foreach (object val in row)
                            {
                                Console.Write($"{val}\t");
                            }
                            Console.WriteLine();
                        }
                    }

                    // Başvurulan alandan belirli bir değeri alın
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Referans adresini gösterin
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ReferredAreaDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReferredArea: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


