---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner özelliği. İlk çalışma sayfasının özel değişkenler içerip içermediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

İlk çalışma sayfasının özel değişkenler içerip içermediğini gösterir.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen WorkbookDesigner.VariablesWorksheetName özelliğini kullanın. Bu özellik Eylül 2025'ten itibaren 3 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Bir WorkbookDesigner örneği oluşturun
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // ContainsVariables özelliğinin mevcut değerini gösterin
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // ContainsVariables özelliğini true olarak ayarlayın
                designer.ContainsVariables = true;

                // Güncellenmiş değeri gösterin
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Sonucu kaydet
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


