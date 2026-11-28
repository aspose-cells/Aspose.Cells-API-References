---
title: "WorkbookDesigner.LineByLine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner özelliği. Akıllı işaretçinin satır satır işlenip işlenmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Akıllı işaretçinin satır satır işlenip işlenmediğini gösterir.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### Açıklamalar

Varsayılan değer true'dur. False ise, şablon dosyası "_CellsSmartMarkers" olarak adlandırılmış bir aralık içermelidir.

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine, aralık akıllı işaretçileri kullanın. Bu özellik Temmuz 2025'ten itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyLineByLineDemo
    {
        public static void Run()
        {
            // Akıllı işaretçilerle örnek bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Çalışma sayfasında akıllı işaretçileri ayarlayın
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // Örnek veri oluştur
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // LineByLine false olarak ayarlandığında işle.
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // Sonucu kaydet
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // Demonstrasyon için basit veri sınıfı
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


