---
title: "DataSorter.AddKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataSorter-metod. Lägger till sorterat kolumnindex och sorteringsordning"
type: docs
url: /sv/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Lägger till sorterat kolumnindex och sorteringsordning.

```csharp
public void AddKey(int key, SortOrder order)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | Int32 | Den sorterade kolumnindexen (absolut position, kolumn A är 0, B är 1, ...) |
| ordning | SortOrder | Sorteringsordningen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Lägg till sorteringsnyckel för kolumn B (index 1) med stigande ordning
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Sortera dataområde (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Skriv ut sorterade värden
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### Se även

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | Int32 | Den sorterade kolumnindexen (absolut position, kolumn A är 0, B är 1, ...) |
| ordning | SortOrder | Sorteringsordningen. |
| customList | String | Den anpassade sorteringslistan. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata att sortera
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Skapa datasortering och lägg till anpassad sorteringsnyckel
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Sortera data
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | Int32 | Den sorterade kolumnindexen (absolut position, kolumn A är 0, B är 1, ...) |
| typ | SortOnType | Den sorterade värdetypen. |
| ordning | SortOrder | Sorteringsordningen. |
| customList | Object | Den anpassade sorteringslistan. |

### Anmärkningar

Om typen är SortOnType.CellColor eller SortOnType.FontColor, är customList en färg.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Skapa en datasortering
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // Anropa AddKey med parametrarna: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Definiera intervallet att sortera
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Sortera data
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | Int32 | Den sorterade kolumnindexen (absolut position, kolumn A är 0, B är 1, ...) |
| ordning | SortOrder | Sorteringsordningen. |
| customList | String[] | Den anpassade sorteringslistan. |

### Se även

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


