---
title: "Sınıf PivotFieldCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotFieldCollection sınıfı. Pivot tablonun farklı bölgelerindeki tüm PivotField nesnelerinin bir koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldcollection/
---
## PivotFieldCollection class

Pivot tablo'nun farklı bölgelerindeki tüm PivotField nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class PivotFieldCollection : CollectionBase<PivotField>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotfieldcollection/item/) { get; } | Belirli indeksteki PivotField nesnesini alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Type](../../aspose.cells.pivot/pivotfieldcollection/type/) { get; } | PivotFields tipini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotfieldcollection/add/)(PivotField) | Belirli PivotFields türüne bir PivotField nesnesi ekler. |
| [AddByBaseIndex](../../aspose.cells.pivot/pivotfieldcollection/addbybaseindex/)(int) | Belirli PivotFields türüne bir PivotField nesnesi ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotField, IComparer&lt;PivotField&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotField, IComparer&lt;PivotField&gt;) |  |
| [Clear](../../aspose.cells.pivot/pivotfieldcollection/clear/#clear)() | PivotFieldCollection'ın tüm alanlarını temizle (2 yöntem) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotField) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotField[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotField[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotField[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotField&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotField&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotField&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotField&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotField, int, int) |  |
| [Insert](../../aspose.cells.pivot/pivotfieldcollection/insert/)(int, PivotField) | Belirli bir indekse bir pivot alanı ekle. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotField, int, int) |  |
| [Move](../../aspose.cells.pivot/pivotfieldcollection/move/)(int, int) | PivotField'ı mevcut konumdan hedef konuma taşır |
| [Remove](../../aspose.cells.pivot/pivotfieldcollection/remove/)(PivotField) | Alanı mevcut bölgeden kaldırır. |
| [RemoveAt](../../aspose.cells.pivot/pivotfieldcollection/removeat/#removeat)(int) | Alanı indeksine göre kaldırır. Yalnızca filtre, satır, sütun, veri bölgesi için. (2 yöntem) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionDemo
    {
        public static void PivotFieldCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Grape";
            worksheet.Cells[2, 0].Value = "Blueberry";
            worksheet.Cells[3, 0].Value = "Kiwi";
            worksheet.Cells[4, 0].Value = "Cherry";
            worksheet.Cells[5, 0].Value = "Grape";
            worksheet.Cells[6, 0].Value = "Blueberry";
            worksheet.Cells[7, 0].Value = "Kiwi";
            worksheet.Cells[8, 0].Value = "Cherry";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Çalışma sayfasına bir pivot tablo ekle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // RowFields koleksiyonuna erişin
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Satır alanlarının sayısını göster
            Console.WriteLine("Row Fields Count: " + rowFields.Count);

            // İlk satır alanına erişin ve adını görüntüleyin
            PivotField firstRowField = rowFields[0];
            Console.WriteLine("First Row Field Name: " + firstRowField.Name);

            // Temel indeksle yeni bir alan ekleyin
            int newFieldIndex = rowFields.AddByBaseIndex(1); // Adding the "Year" field to the row area
            Console.WriteLine("New Field Index: " + newFieldIndex);

            // RowFields koleksiyonundaki tüm alanları temizleyin
            rowFields.Clear();
            Console.WriteLine("Row Fields Count after Clear: " + rowFields.Count);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotField](../pivotfield/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


