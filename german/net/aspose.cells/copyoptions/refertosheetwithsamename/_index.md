---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions property. In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln sich auf die Quellarbeitsmappe beziehen. In einigen Fällen kann der Benutzer jedoch benötigen, dass die kopierten Formeln sich auf Arbeitsblätter mit demselben Namen in derselben Arbeitsmappe beziehen, zum Beispiel wenn diese Arbeitsblätter bereits vor diesem Kopiervorgang kopiert wurden; dann sollte diese Eigenschaft auf true gesetzt bleiben."
type: docs
url: /de/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

In MS Excel, wenn Formeln, die sich auf andere Arbeitsblätter beziehen, beim Kopieren eines Arbeitsblatts in ein anderes kopiert werden, sollten die kopierten Formeln auf die Quellarbeitsmappe verweisen. In einigen Situationen muss der Benutzer jedoch, dass die kopierten Formeln auf Arbeitsblätter mit demselben Namen in derselben Arbeitsmappe verweisen, zum Beispiel wenn diese Arbeitsblätter bereits vor diesem Kopiervorgang kopiert wurden; dann sollte diese Eigenschaft auf true gesetzt bleiben.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // Erstelle eine Vorlage-Arbeitsmappe mit Beispieldaten
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // Erstelle Ausgabearbeitsmappe
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // Kopiere Arbeitsblätter mit aktiviertem ReferToSheetWithSameName
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // Überprüfe, ob die Formel das korrekte Blatt referenziert
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


