---
title: "Workbook-klass"
linktitle: "Workbook"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Workbook-klass. Inkapslar objektet som representerar en arbetsbok i Go."
type: docs
weight: 200
url: /sv/go-cpp/workbook/
---

## Workbook class

Representerar ett rotobjekt för att skapa ett Excel‑kalkylblad.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewWorkbook](./newworkbook/) | Initierar en ny instans av Workbook-klassen. |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Initierar en ny instans av Workbook-klassen. |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | Initierar en ny tom instans av Workbook-klassen med alternativ |
| [NewWorkbook_String](./newworkbook_string/) | Initierar en ny instans av Workbook-klassen och öppnar en fil. |
| [NewWorkbook_Stream](./newworkbook_stream/) | Initierar en ny instans av Workbook-klassen och öppnar en ström. |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Initierar en ny instans av Workbook-klassen och öppnar en fil. |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | Initierar en ny instans av Workbook-klassen och öppnar strömmen. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetSettings](./getsettings/) | Representerar arbetsboksinställningarna. |
| [ParseFormulas](./parseformulas/) | Analyserar alla formler som inte har analyserats när de laddades från mallfilen eller sattes i en cell. |
| [StartAccessCache](./startaccesscache/) | Startar sessionen som använder cache för att komma åt data. |
| [CloseAccessCache](./closeaccesscache/) | Stänger sessionen som använder cache för att komma åt data. |
| [Save_String_SaveFormat](./save_string_saveformat/) | Sparar arbetsboken till disken. |
| [Save_String](./save_string/) | Spara arbetsboken till disken. |
| [Save_String_SaveOptions](./save_string_saveoptions/) | Sparar arbetsboken till disken. |
| [Save_SaveFormat](./save_saveformat/) | Sparar arbetsboken till strömmen. |
| [Save_SaveOptions](./save_saveoptions/) | Sparar arbetsboken till strömmen. |
| [SaveToStream](./savetostream/) | Sparar Excel-filen till ett MemoryStream-objekt som en Excel97-2003 xls-fil och returnerar den. |
| [GetWorksheets](./getworksheets/) | Hämtar WorksheetCollection-samlingen i kalkylbladet. |
| [IsLicensed](./islicensed/) | Anger om licensen är inställd. |
| [RemoveUnusedStyles](./removeunusedstyles/) | Ta bort alla oanvända stilar. |
| [CreateStyle](./createstyle/) | Skapar en ny stil. |
| [CreateStyle_Bool](./createstyle_bool/) | Skapar en ny stil. |
| [CreateBuiltinStyle](./createbuiltinstyle/) | Skapar inbyggd stil av given typ. |
| [CreateCellsColor](./createcellscolor/) | Skapar ett CellsColor-objekt. |
| [Replace_String_String](./replace_string_string/) | Ersätter en cells värde med en ny sträng. |
| [Replace_String_Int](./replace_string_int/) | Ersätter en cells värde med ett nytt heltal. |
| [Replace_String_Double](./replace_string_double/) | Ersätter en cells värde med ett nytt dubbelvärde. |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | Ersätter en cells värde med en ny strängarray. |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | Ersätter cellers värden med en heltalsarray. |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | Ersätter cellers värden med en dubbelarray. |
| [Replace_Bool_Object](./replace_bool_object/) | Ersätter cellers värden med nya data. |
| [Replace_Int_Object](./replace_int_object/) | Ersätter cellers värden med nya data. |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | Ersätter en cells värde med en ny sträng. |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | Kopierar ett annat Workbook-objekt. |
| [Copy_Workbook](./copy_workbook/) | Kopierar data från ett käll-Workbook-objekt. |
| [Combine](./combine/) | Kombinerar ett annat Workbook-objekt. |
| [GetColors](./getcolors/) | Returnerar färger i paletten för kalkylbladet. |
| [GetStyleInPool](./getstyleinpool/) | Hämtar stilen i stilpoolen. Alla stilar i arbetsboken samlas i en pool. Det finns bara ett enkelt referensindex i cellerna. |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | Hämtar antalet stilar i stilpoolen. |
| [GetFonts](./getfonts/) | Hämtar alla teckensnitt i stilpoolen. |
| [GetNamedStyle](./getnamedstyle/) | Hämtar den namngivna stilen i stilpoolen. |
| [MergeNamedStyles](./mergenamedstyles/) | Slår ihop namngivna stilar från den andra Excel-filen. |
| [ChangePalette](./changepalette/) | Ändrar paletten för kalkylbladet på det angivna indexet. |
| [IsColorInPalette](./iscolorinpalette/) | Kontrollerar om en färg finns i paletten för kalkylbladet. |
| [CalculateFormula](./calculateformula/) | Beräknar resultatet av formler. |
| [CalculateFormula_Bool](./calculateformula_bool/) | Beräknar resultatet av formler. |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | Beräknar formler i den här arbetsboken. |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | Uppdaterar dynamiska array-formler (sprider till nytt område av intilliggande celler enligt aktuell data) Andra formler i arbetsboken kommer inte att beräknas rekursivt även om de användes av dynamiska array-formler. |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | Uppdaterar dynamiska array-formler (sprider till nytt område av intilliggande celler enligt aktuell data) |
| [GetDefaultStyle](./getdefaultstyle/) | Hämtar eller anger standard‑Style‑objektet för arbetsboken. |
| [SetDefaultStyle](./setdefaultstyle/) | Hämtar eller anger standard‑Style‑objektet för arbetsboken. |
| [GetMatchingColor](./getmatchingcolor/) | Hitta bäst matchande Color i aktuell palette. |
| [IsDigitallySigned](./isdigitallysigned/) | Indikerar om detta kalkylblad är digitalt signerat. |
| [SetEncryptionOptions](./setencryptionoptions/) | Ställ in krypteringsalternativ. |
| [Protect](./protect/) | Skyddar en arbetsbok. |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | Skyddar en delad arbetsbok. |
| [Unprotect](./unprotect/) | Avskyddar en arbetsbok. |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Avskyddar en delad arbetsbok. |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Anger om struktur eller fönster är skyddade med lösenord. |
| [RemoveMacro](./removemacro/) | Tar bort VBA/makro från detta kalkylblad. |
| [GetVbaProject](./getvbaproject/) | Hämtar VbaProject i ett kalkylblad. |
| [RemoveDigitalSignature](./removedigitalsignature/) | Tar bort digital signatur från detta kalkylblad. |
| [AcceptAllRevisions](./acceptallrevisions/) | Accepterar alla spårade ändringar i arbetsboken. |
| [GetHasMacro](./gethasmacro/) | Anger om detta kalkylblad innehåller makro/VBA. |
| [GetHasRevisions](./gethasrevisions/) | Hämtar om arbetsboken har några spårade ändringar |
| [GetFileName](./getfilename/) | Hämtar och anger det aktuella filnamnet. |
| [SetFileName](./setfilename/) | Hämtar och anger det aktuella filnamnet. |
| [GetDataSorter](./getdatasorter/) | Hämtar ett DataSorter-objekt för att sortera data. |
| [GetThemeColor](./getthemecolor/) | Hämtar temafärg. |
| [SetThemeColor](./setthemecolor/) | Anger temafärgen |
| [GetTheme](./gettheme/) | Hämtar temats namn. |
| [CustomTheme](./customtheme/) | Anpassar temat. |
| [CopyTheme](./copytheme/) | Kopierar temat från en annan arbetsbok. |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Uppdaterar definitionen av anpassade funktioner. |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | Om denna arbetsbok innehåller externa länkar till andra datakällor,Aspose.Cells kommer att försöka hämta den senaste datan från angivna källor. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returnerar en DocumentProperty-samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returnerar en DocumentProperty-samling som representerar alla anpassade dokumentegenskaper i kalkylbladet. |
| [GetFileFormat](./getfileformat/) | Hämtar och anger filformatet. |
| [SetFileFormat](./setfileformat/) | Hämtar och anger filformatet. |
| [GetHasCustomFunction](./gethascustomfunction/) | Detekterar om det finns anpassade funktioner som används i denna arbetsbok,såsom i cellens formel, i definierade namn... |
| [GetInterruptMonitor](./getinterruptmonitor/) | Hämtar och anger avbrottsmotorn. |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | Hämtar och anger avbrottsmotorn. |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | Ställer in avbrottsmontorn. |
| [GetContentTypeProperties](./getcontenttypeproperties/) | Hämtar listan med ContentTypeProperty-objekt i arbetsboken. |
| [GetCustomXmlParts](./getcustomxmlparts/) | Representerar en anpassad XML‑datalagringsdel (anpassad XML‑data inom ett paket). |
| [GetDataMashup](./getdatamashup/) | Hämtar mashup-data. |
| [GetRibbonXml](./getribbonxml/) | Hämtar och anger XML-filen som definierar Ribbon UI. |
| [SetRibbonXml](./setribbonxml/) | Hämtar och anger XML-filen som definierar Ribbon UI. |
| [GetAbsolutePath](./getabsolutepath/) | Hämtar och anger den absoluta sökvägen till filen. |
| [SetAbsolutePath](./setabsolutepath/) | Hämtar och anger den absoluta sökvägen till filen. |
| [GetDataConnections](./getdataconnections/) | Hämtar ExternalConnection-samlingen. |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | Importerar/Uppdaterar en XML-datafil i arbetsboken. |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | Importerar/Uppdaterar en XML-datafil i arbetsboken. |
| [ExportXml_String_String](./exportxml_string_string/) | Exporterar XML-data som är länkad via den angivna XML-kartan. |
| [ExportXml_String](./exportxml_string/) | Exportera XML-data. |
| [SetDigitalSignature](./setdigitalsignature/) | Ställer in digital signatur för en kalkylbladsfil (Excel2007 och senare). |
| [AddDigitalSignature](./adddigitalsignature/) | Lägger till digital signatur i en OOXML-kalkylbladsfil (Excel2007 och senare). |
| [GetDigitalSignature](./getdigitalsignature/) | Hämtar digital signatur från fil. |
| [RemovePersonalInformation](./removepersonalinformation/) | Tar bort personlig information. |
| [GetDataModel](./getdatamodel/) | Hämtar datamodellen i arbetsboken. |
| [RefreshAll](./refreshall/) | Uppdaterar länkade former, alla pivottabeller och diagram med pivottabellskälla. |
| [Dispose](./dispose/) | Utför applikationsdefinierade uppgifter som är kopplade till frigöring, släppande eller återställning av ohanterade resurser. |
