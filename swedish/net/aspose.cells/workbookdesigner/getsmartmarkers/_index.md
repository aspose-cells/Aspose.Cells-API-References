---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-metod. Returnerar en samling av smarta markörer i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Returnerar en samling av smart markers i ett kalkylblad.

```csharp
public string[] GetSmartMarkers()
```

### Returvärde

En samling av smarta markörer

### Anmärkningar

En string-array skapas vid varje anrop. Arrayen sorteras och duplicerade värden tas bort.

### Exempel

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // Skapa en exempelmallfil i minnet
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // Lägg till smarta markörer i mallen
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // Spara mallen till minnesström
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // Initiera WorkbookDesigner med mallen
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // Hämta och visa smarta markörer
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // Förbered datakälla
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // Ange datakälla och bearbeta
            designer.SetDataSource(data);
            designer.Process();
            
            // Spara resultatet
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


