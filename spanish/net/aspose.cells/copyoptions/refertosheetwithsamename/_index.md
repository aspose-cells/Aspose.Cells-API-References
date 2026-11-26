---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CopyOptions. En ms excel, al copiar fórmulas que hacen referencia a otras hojas de cálculo mientras se copia una hoja a otra, las fórmulas copiadas deben referirse al libro de origen. Sin embargo, en algunas situaciones el usuario puede necesitar que las fórmulas copiadas se refieran a hojas con el mismo nombre en el mismo libro, como cuando esas hojas ya se han copiado antes de esta operación de copia; entonces esta propiedad debe mantenerse en true."
type: docs
url: /es/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

En MS Excel, al copiar fórmulas que hacen referencia a otras hojas de cálculo mientras se copia una hoja a otra, las fórmulas copiadas deben referirse al libro de origen. Sin embargo, en algunas situaciones el usuario puede necesitar que las fórmulas copiadas hagan referencia a hojas con el mismo nombre en el mismo libro, como cuando esas hojas ya fueron copiadas antes de esta operación de copia, entonces esta propiedad debe mantenerse como true.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // Cree un libro plantilla con datos de ejemplo
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // Cree el libro de salida
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // Copie las hojas de cálculo con ReferToSheetWithSameName habilitado
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // Verifique que la fórmula haga referencia a la hoja correcta
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


