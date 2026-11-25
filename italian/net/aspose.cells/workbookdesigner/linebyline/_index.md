---
title: "WorkbookDesigner.LineByLine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookDesigner. Indica se l'elaborazione dello smart marker avviene riga per riga"
type: docs
url: /it/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Indica se l'elaborazione dello smart marker avviene riga per riga.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### Osservazioni

Il valore predefinito è true. Se False, il file modello deve contenere un intervallo denominato "_CellsSmartMarkers".

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare smart marker di intervallo. Questa proprietà sarà rimossa tra 12 mesi a partire da luglio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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
            // Crea un workbook di esempio con smart marker
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Configura gli smart marker nel foglio di lavoro
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // Crea dati di esempio
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // Elabora con LineByLine impostato su false
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // Salva il risultato
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // Classe dati semplice per dimostrazione
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


