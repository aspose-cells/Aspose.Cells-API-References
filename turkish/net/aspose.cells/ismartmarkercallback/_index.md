---
title: "Arayüz ISmartMarkerCallBack"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ISmartMarkerCallBack arayüzü. Akıllı işaretçi işleme geri çağırma arayüzünü temsil eder"
type: docs
url: /tr/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

Smartmarker işleme geri çağırma arayüzünü temsil eder.

```csharp
public interface ISmartMarkerCallBack
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Akıllı işaretçi işlemek için geri çağırma. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // ISmartMarkerCallBack arayüzündeki Process metodunu uygulama
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Process metodunun örnek uygulaması
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // Yeni bir WorkbookDesigner örneği oluşturun
            WorkbookDesigner designer = new WorkbookDesigner();
            // Akıllı işaretçileri içeren bir şablon dosyasını açın
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Geri çağırma arayüzünü ayarlayın
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Veri kaynağından verilerinizi başlatın
            // Gösterim amacıyla basit bir DataTable kullanacağız
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // DataTable'ı veri kaynağı olarak ayarlayın
            designer.SetDataSource(dataTable);

            // Akıllı işaretçileri işleyerek verileri çalışma sayfalarına doldurun
            designer.Process(true);

            // Excel dosyasını kaydet.
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


