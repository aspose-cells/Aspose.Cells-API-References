---
title: Protect
second_title: Aspose.Cells för .NET API-referens
description: Skyddar kalkylblad.
type: docs
weight: 770
url: /sv/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Skyddar kalkylblad.

```csharp
public void Protect(ProtectionType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | ProtectionType | Skyddstyp. |

### Anmärkningar

Denna metod skyddar kalkylblad utan lösenord. Det kan skydda kalkylblad i alla versioner av Excel-fil.

### Se även

* enum [ProtectionType](../../protectiontype)
* class [Worksheet](../../worksheet)
* namnutrymme [Aspose.Cells](../../worksheet)
* hopsättning [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Skyddar kalkylblad.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | ProtectionType | Skyddstyp. |
| password | String | Lösenord. |
| oldPassword | String | Om kalkylbladet redan är skyddat av ett lösenord, vänligen ange det gamla lösenordet. Annars kan du ställa in ett nollvärde eller en tom sträng för denna parameter. |

### Anmärkningar

Denna metod kan skydda kalkylblad i alla versioner av Excel-fil.

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook excel = new Workbook("template.xlsx");
//Åtkomst till det första kalkylbladet i Excel-filen
Worksheet worksheet = excel.Worksheets[0];
//Skydda kalkylbladet med ett lösenord
worksheet.Protect(ProtectionType.All, "aspose", null);
//Spara den modifierade Excel-filen i standardformat (det vill säga Excel 20003).
excel.Save("output.xls");
//Stänger filströmmen för att frigöra alla resurser

[Visual Basic]

'Skapa en filström som innehåller Excel-filen som ska öppnas
Dim fstream As FileStream = New FileStream("book1.xls", FileMode.Open)
'Instantiera ett arbetsboksobjekt och öppna Excel-filen via filströmmen
Dim excel As Workbook = New Workbook(fstream)
'Åtkomst till det första kalkylbladet i Excel-filen
Dim worksheet As Worksheet = excel.Worksheets(0)
'Skydda arbetsbladet med ett lösenord
worksheet.Protect(ProtectionType.All, "aspose", DBNull.Value.ToString())
'Spara den modifierade Excel-filen i standardformat (det vill säga Excel 20003).
excel.Save("output.xls")
'Stänger filströmmen för att frigöra alla resurser
fstream.Close()

```

### Se även

* enum [ProtectionType](../../protectiontype)
* class [Worksheet](../../worksheet)
* namnutrymme [Aspose.Cells](../../worksheet)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->