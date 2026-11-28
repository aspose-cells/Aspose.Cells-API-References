---
title: "Class WorkbookDesigner"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WorkbookDesigner sınıfı. Tasarımcı elektronik tablosunu temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Tasarımcı çalışma sayfasını temsil eden nesneyi kapsüller.

```csharp
public class WorkbookDesigner
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Yeni bir `WorkbookDesigner` sınıfı örneği başlatır. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Yeni bir `WorkbookDesigner` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Formüllerin hesaplanıp hesaplanmayacağını gösterir. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Smartmarker işleme geri çağırma arayüzünü alır ve ayarlar. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) İlk çalışma sayfasının özel değişkenler içerip içermediğini gösterir. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | Üstbilgi/altbilginin akıllı işaretçiler içerip içermediğini ve birlikte işlenmesi gerektiğini gösterir. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Akıllı işaretçinin satır satır işlenip işlenmeyeceğini gösterir. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Alt toplam satırıyla formüllerin tekrarlanıp tekrarlanmadığını gösterir. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Veri kaynağının sıralanıp sıralanmadığını gösterir. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | Eğer TRUE ise, değer "" olduğunda Null eklenecektir; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Değişken akıllı işaretçileri içeren çalışma sayfasının adını alır ve ayarlar. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Alır ve ayarlar [`Workbook`](./workbook/) nesnesini. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Tüm veri kaynaklarını temizler. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Bir elektronik tabloda akıllı işaretçilerin bir koleksiyonunu döndürür. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Obsolete.**) Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Bir DataSet nesnesinin veri kaynağını ayarlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Bir DataTable nesnesinin veri kaynağını ayarlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Bir DataView nesnesinin veri kaynağını ayarlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Bir OleDbConnection nesnesinin veri kaynağını ayarlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Bir SqlConnection nesnesinin veri kaynağını ayarlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Bir DataView nesnesinin veri kaynağını ayarlar ve onu bir veri kaynağı adına bağlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Bir [`ICellsDataTable`](../icellsdatatable/) nesnesinin veri kaynağını ayarlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Veri bağlamayı bir değişkene ayarlar. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Bir IDataReader nesnesinin veri kaynağını ayarlar. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | JSON dize değerini akıllı işaretçilerin veri kaynağı olarak ayarla. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerDemo
    {
        public static void WorkbookDesignerExample()
        {
            // WorkbookDesigner nesnesi oluştur
            WorkbookDesigner wd = new WorkbookDesigner();

            // Akıllı işaretçileri içeren şablon dosyasını aç
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Veri kaynağından verilerinizi başlatın
            DataSet ds = new DataSet();
            // Veri kümesine veri ekle (bu sadece bir örnek, gerçek veri kaynağıyla değiştirin)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Veri kümesini veri kaynağı olarak ayarla
            wd.SetDataSource(ds);

            // Akıllı işaretçileri işleyerek verileri çalışma sayfalarına doldurun
            wd.Process(true);

            // Excel dosyasını kaydet.
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Diğer özellikleri gösterme
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Veri kaynağını temizle
            wd.ClearDataSource();

            // Farklı yöntemlerle veri kaynağını ayarla
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Akıllı işaretçileri tekrar işle
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Excel dosyasını tekrar kaydet
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


