---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner özelliği. Değişken akıllı işaretçiyi içeren çalışma sayfasının adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Değişken akıllı işaretçileri içeren çalışma sayfasının adını alır ve ayarlar.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();

                // "Variables" adlı bir çalışma sayfası ekleyerek özelliği gösterin
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Bir WorkbookDesigner örneği oluşturun
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Mevcut VariablesWorksheetName değerini gösterin
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // VariablesWorksheetName için yeni bir değer ayarlayın
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Akıllı işaretçileri içeren başka bir çalışma sayfası ekleyin
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Akıllı işaretçileri işleyin
                designer.Process();

                // Çalışma kitabını kaydedin
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
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


