---
title: "MetadataOptions.MetadataType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MetadataOptions. تحصل وتضبط نوع البيانات الوصفية التي يتم تحميلها"
type: docs
url: /ar/net/aspose.cells.metadata/metadataoptions/metadatatype/
---
## MetadataOptions.MetadataType property

يحصل ويضبط نوع البيانات الوصفية التي يتم تحميلها.

```csharp
public MetadataType MetadataType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsPropertyMetadataTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Confidential Data");

            MetadataOptions encryptOptions = new MetadataOptions(MetadataType.Encryption);
            Console.WriteLine("Encryption MetadataType: " + encryptOptions.MetadataType);
            encryptOptions.Password = "secret";
            encryptOptions.KeyLength = 128;

            XlsSaveOptions saveOptions = new XlsSaveOptions();
            // خيارات التشفير المطبقة عبر إعدادات دفتر العمل
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, encryptOptions.KeyLength);
            workbook.Settings.Password = encryptOptions.Password;

            workbook.Save("PropertyMetadataTypeDemo.xls", saveOptions);

            MetadataOptions decryptOptions = new MetadataOptions(MetadataType.Decryption);
            Console.WriteLine("Decryption MetadataType: " + decryptOptions.MetadataType);
            decryptOptions.Password = "secret";

            LoadOptions loadOptions = new LoadOptions(LoadFormat.Excel97To2003);
            loadOptions.Password = decryptOptions.Password;
            
            Workbook decryptedWorkbook = new Workbook("PropertyMetadataTypeDemo.xls", loadOptions);
            Console.WriteLine("Decrypted value: " + decryptedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


