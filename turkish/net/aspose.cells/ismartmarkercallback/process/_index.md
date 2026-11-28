---
title: "ISmartMarkerCallBack.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ISmartMarkerCallBack yöntemi. Akıllı işaretçi işleme için geri arama"
type: docs
url: /tr/net/aspose.cells/ismartmarkercallback/process/
---
## ISmartMarkerCallBack.Process method

Akıllı işaretçi işlemek için geri çağırma.

```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | Int32 | Sayfa indeksi. |
| rowIndex | Int32 | Satır indeksi. |
| colIndex | Int32 | Sütun indeksi. |
| tableName | String | Akıllı işaretçinin tablo adı. |
| columnName | String | Akıllı işaretçinin tablo adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo : ISmartMarkerCallBack
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo callback = 
                new ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo();

            try
            {
                // Process yöntemini örnek parametrelerle çağır
                callback.Process(0, 5, 3, "Products", "ProductName");
                
                Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
                
                // Etkiyi göstermek için bir değer ayarla
                worksheet.Cells[5, 3].PutValue("ProcessedValue");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            
            workbook.Save("ISmartMarkerCallBackProcessDemo.xlsx");
        }

        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Process yönteminin uygulanması
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


