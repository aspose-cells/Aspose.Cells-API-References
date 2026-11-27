---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Lägger till en tilläggsfunktion i arbetsboken"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Lägger till tilläggsfunktion i arbetsboken

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| addInFile | String | filen innehåller tilläggsfunktionerna |
| functionName | String | namnet på tilläggsfunktionen |
| lib | Boolean | om den angivna tilläggsfilen finns i katalogen eller underkatalogen för Workbook Add-In-biblioteket. Denna flagga aktiveras och gör skillnad när den angivna addInFile är en relativ sökväg: true betyder att sökvägen är relativ till Add-In-biblioteket och false betyder att sökvägen är relativ till denna arbetsbok. |

### Returvärde

ID för den data som innehåller den angivna tilläggsfunktionen

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Hämta det första kalkylbladet
            Worksheet sheet = wb.Worksheets[0];
            
            // Ange exempel på filsökvägar (de måste finnas i din miljö)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // Registrera tilläggsfunktioner med olika parametrar
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // Använd de registrerade funktionerna i celler
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // Spara arbetsboken
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Lägger till tilläggsfunktion i arbetsboken

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| id | Int32 | ID för den data som innehåller tilläggsfunktioner, kan erhållas genom det första anropet av `RegisterAddInFunction` för samma tilläggsfil. |
| functionName | String | namnet på tilläggsfunktionen |

### Returvärde

URL för tilläggsfilen som innehåller tilläggsfunktioner

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Registrera den första tilläggsfunktionen och hämta dess ID
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // Registrera den andra tilläggsfunktionen med samma ID
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Använd de registrerade funktionerna i formler
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // Spara arbetsboken
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


