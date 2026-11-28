---
title: "Sınıf HtmlTableLoadOptionCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlTableLoadOptionCollection sınıfı. HTML içe aktarılırken tablo seçeneklerini temsil eder."
type: docs
url: /tr/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

HTML içe aktarılırken tablo seçeneklerini temsil eder.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | Belirtilen indeksteki [`HtmlTableLoadOption`](../htmltableloadoption/) öğesini alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | İçe aktarılan tablolardan liste nesneleri oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) Bu koleksiyona bir HtmlTableLoadOption ekler. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | Listeye bir HtmlTableLoadOption ekle. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | Listeye bir HtmlTableLoadOption ekle. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | Listeye bir HtmlTableLoadOption ekle. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | Listeye bir HtmlTableLoadOption ekle. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | Listeye bir HtmlTableLoadOption ekle. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | Listeye bir HtmlTableLoadOption ekle. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | Bu koleksiyona bir HtmlTableLoadOption ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();

            // HtmlLoadOptions oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // HtmlTableLoadOptionCollection örneğine erişin
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // TableToListObject özelliğini ayarlayın
            tableLoadOptions.TableToListObject = true;

            // Tablo indeksine göre yeni bir HtmlTableLoadOption ekleyin
            int index1 = tableLoadOptions.Add(0);

            // Tablo kimliğine göre yeni bir HtmlTableLoadOption ekleyin
            int index2 = tableLoadOptions.Add("tableId");

            // Tablo indeksi ve hedef sayfa indeksiyle yeni bir HtmlTableLoadOption ekleyin
            int index3 = tableLoadOptions.Add(1, 1);

            // Tablo kimliği ve hedef sayfa indeksiyle yeni bir HtmlTableLoadOption ekleyin
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Tablo indeksi, hedef sayfa indeksi ve özgün sayfa indeksiyle yeni bir HtmlTableLoadOption ekleyin
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Tablo kimliği, hedef sayfa indeksi ve özgün sayfa indeksiyle yeni bir HtmlTableLoadOption ekleyin
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Belirli bir indeksdeki HtmlTableLoadOption'a erişin
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // HtmlTableLoadOption'ın özelliklerini ayarlayın
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Yükleme seçeneklerini kullanarak bir HTML dosyasını çalışma kitabına yükleyin
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


