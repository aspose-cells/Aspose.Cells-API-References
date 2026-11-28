---
title: "DataModel.Tables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModel özelliği. Veri modelindeki tüm tabloları alır"
type: docs
url: /tr/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Veri modelindeki tüm tabloları alır.

```csharp
public DataModelTableCollection Tables { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class DataModelPropertyTablesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Veri modeline erişin
            DataModel dataModel = wb.DataModel;
            
            // Tablolar koleksiyonunu alın ve sayısını gösterin
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // Veri modeli içeren örnek çalışma kitabını yükleyin
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // Tablolar koleksiyonuna erişin
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // Tablolar arasında yineleme yapın
                foreach (DataModelTable table in tables)
                {
                    Console.WriteLine($"Table name: {table.Name}");
                }
            }
            else
            {
                Console.WriteLine($"Sample file '{sourceFile}' not found. Create an Excel file with data model to see tables information.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


