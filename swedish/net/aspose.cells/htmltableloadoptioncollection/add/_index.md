---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOptionCollection-metod. Lägger till en HtmlTableLoadOption i den här samlingen"
type: docs
url: /sv/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Lägger till ett HtmlTableLoadOption i den här samlingen.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | HtmlTableLoadOption | en HtmlTableLoadOption |

### Returvärde

index för det tillagda objektet

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället metoden AddTableLoadOption(). Denna metod kommer att tas bort 6 månader senare, från och med december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Lägg till tabellens laddningsalternativ
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Läs in arbetsbok med alternativ
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Spara utdata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Lägg till ett HtmlTableLoadOption i listan.

```csharp
public int Add(int tableIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableIndex | Int32 | Tabellindex |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Kom åt HtmlTableLoadOptionCollection-instansen
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Lägg till ett nytt HtmlTableLoadOption med tabellindex
            int index = tableLoadOptions.Add(0);

            // Åtkomst till den tillagda HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // Skapa en arbetsbok och läs in HTML med alternativ
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Lägg till ett HtmlTableLoadOption i listan.

```csharp
public int Add(string tableId)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableId | String | Tabell-ID |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Kom åt HtmlTableLoadOptionCollection-instansen
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Lägg till ett nytt HtmlTableLoadOption med tabell-ID
            int index = tableLoadOptions.Add("mainTable");

            // Åtkomst till den tillagda HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // Skapa arbetsbok och läs in HTML med alternativ
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Lägg till ett HtmlTableLoadOption i listan.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableIndex | Int32 | Tabellindex |
| targetSheetIndex | Int32 | Målindex för kalkylblad i Excel |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Lägg till tabeller efter index med målbladets index
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // Läs in HTML-fil med de angivna alternativen
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Lägg till ett HtmlTableLoadOption i listan.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableId | String | Tabell-ID |
| targetSheetIndex | Int32 | Målindex för kalkylblad i Excel |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Kom åt HtmlTableLoadOptionCollection-instansen
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Lägg till ett nytt HtmlTableLoadOption med tabell-ID och målbladindex
            int index = tableLoadOptions.Add("tableId", 1);

            // Skapa en arbetsbok och läs in HTML med alternativ
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Lägg till ett HtmlTableLoadOption i listan.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableIndex | Int32 | Tabellindex |
| targetSheetIndex | Int32 | Målindex för kalkylblad i Excel |
| originalSheetIndex | Int32 | Det ursprungliga indexet för kalkylbladet i HTML |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Åtkomst till HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Lägg till en tabell med index 1, målbladets index 1 och ursprungligt bladindex 0
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // Skapa en arbetsbok och läs in HTML med alternativ
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Lägg till ett HtmlTableLoadOption i listan.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableId | String | Tabell-ID |
| targetSheetIndex | Int32 | Målindex för kalkylblad i Excel |
| originalSheetIndex | Int32 | Det ursprungliga indexet för kalkylbladet i HTML |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Visa Add-metoden med parametrarna (String, Int32, Int32)
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // Läs in HTML-fil (ersätt med faktisk filsökväg)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


