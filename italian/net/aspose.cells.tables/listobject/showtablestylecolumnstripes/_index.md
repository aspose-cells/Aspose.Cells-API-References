---
title: "ListObject.ShowTableStyleColumnStripes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Indica se la formattazione a strisce di colonna è applicata"
type: docs
url: /it/net/aspose.cells.tables/listobject/showtablestylecolumnstripes/
---
## ListObject.ShowTableStyleColumnStripes property

Indica se la formattazione a strisce di colonna è applicata a.

```csharp
public bool ShowTableStyleColumnStripes { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleColumnStripesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Crea un list object e ottieni il riferimento
            int listObjectIndex = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Imposta la proprietà delle strisce di colonna
            listObject.ShowTableStyleColumnStripes = true;
            
            // Salva la cartella di lavoro
            workbook.Save("ListObjectWithColumnStripes.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with column stripes enabled.");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


