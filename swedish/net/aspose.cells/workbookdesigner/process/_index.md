---
title: "WorkbookDesigner.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-metoden. Bearbetar de smarta markörerna och fyller i värdena för datakällan"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Bearbetar smart markers och fyller i värdena för datakällan.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Intervallet som ska bearbetas |
| isPreserved | Boolean | Sant om den oigenkända smarta markören bevaras. |

### Anmärkningar

OBS: Denna klass är nu föråldrad. Använd i stället Range smarta markörer. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = wb.Worksheets[0];
            
            // Skapa exempeldata i celler
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // Skapa arbetsboksdesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // Skapa JSON-datakälla
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // Bearbeta specifikt intervall med smarta markörer
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // Bearbeta intervallet (true = bearbeta endast detta intervall)
            designer.Process(range, true);
            
            // Spara resultatet
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Bearbetar smart markers och fyller i värdena för datakällan.

```csharp
public void Process()
```

### Exempel

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från mallfil
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Förbered datakälla
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // Ange datakälla och bearbeta
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Bearbetar smart markers och fyller i värdena för datakällan.

```csharp
public void Process(bool isPreserved)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isPreserved | Boolean | Sant om den oigenkända smarta markören bevaras. |

### Exempel

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // Initiera arbetsbok och ladda mall
            Workbook workbook = new Workbook("example.xlsx");
            
            // Skapa exempeldata direkt istället för att ladda från JSON
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // Ställ in smarta markörer
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // Förbered datakällor
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // Bearbeta arbetsboksdesigner
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // Bearbeta med boolesk parameter
            designer.Process(true);
            
            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }

    // Exempeldataklasser
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Bearbetar smart markers och fyller i värdena för datakällan.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Kalkylbladsindex. |
| isPreserved | Boolean | Sant om den oigenkända smarta markören bevaras. |

### Anmärkningar

Denna metod fungerar på kalkylbladsnivå.

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från källfil
            Workbook workbook = new Workbook("example.xlsx");
            
            // Exportera data från kalkylblad till DataTable
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // Skapa arbetsboksdesigner och ställ in datakälla
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // Bearbeta designern med parametrar (Int32, Boolean)
            designer.Process(0, true);

            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


