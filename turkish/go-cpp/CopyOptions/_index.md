---
title: "CopyOptions Sınıfı"
linktitle: "CopyOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CopyOptions sınıfı. Go'da copyoptions'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/copyoptions/
---

## CopyOptions class

Kopyalama seçeneklerini temsil eder.

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | CopyOptions yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetKeepMacros](./getkeepmacros/) | Makroların korunup korunmayacağını belirtir; |
| [SetKeepMacros](./setkeepmacros/) | Makroların korunup korunmayacağını belirtir; |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | Aralığı bitişik aralığa kopyalarken aralıkların genişletilip genişletilmeyeceğini belirtir. |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | Aralığı bitişik aralığa kopyalarken aralıkların genişletilip genişletilmeyeceğini belirtir. |
| [GetCopyNames](./getcopynames/) | İsimlerin kopyalanıp kopyalanmayacağını belirtir. |
| [SetCopyNames](./setcopynames/) | İsimlerin kopyalanıp kopyalanmayacağını belirtir. |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | Formül hedef konum için geçerli değilse, yalnızca değerler kopyalanır. |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | Formül hedef konum için geçerli değilse, yalnızca değerler kopyalanır. |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | Sütun genişliğinin karakter biriminde kopyalanıp kopyalanmayacağını belirtir. |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | Sütun genişliğinin karakter biriminde kopyalanıp kopyalanmayacağını belirtir. |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına başvuran formüller kopyalandığında, kopyalanan formüller kaynak çalışma kitabına başvurmalıdır. Ancak bazı durumlarda kullanıcı, kopyalanan formüllerin aynı çalışma kitabında aynı ada sahip çalışma sayfalarına başvurmasını isteyebilir; örneğin bu çalışma sayfaları bu kopyalama işleminden önce zaten kopyalanmışsa, bu özellik true olarak tutulmalıdır. |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına başvuran formüller kopyalandığında, kopyalanan formüller kaynak çalışma kitabına başvurmalıdır. Ancak bazı durumlarda kullanıcı, kopyalanan formüllerin aynı çalışma kitabında aynı ada sahip çalışma sayfalarına başvurmasını isteyebilir; örneğin bu çalışma sayfaları bu kopyalama işleminden önce zaten kopyalanmışsa, bu özellik true olarak tutulmalıdır. |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | Aynı dosyada aralık kopyalanırken ve grafik kaynak sayfaya başvuruyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceğini, True ise kopyalanan grafiğin veri kaynağının hedef sayfaya başvuracağını ifade eder. |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | Aynı dosyada aralık kopyalanırken ve grafik kaynak sayfaya başvuruyorsa, False kopyalanan grafiğin veri kaynağının değişmeyeceğini, True ise kopyalanan grafiğin veri kaynağının hedef sayfaya başvuracağını ifade eder. |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | Başvurulan çalışma sayfası kopyalanmamışsa hedef çalışma sayfasına başvurulup başvurulmayacağını belirtir. |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | Başvurulan çalışma sayfası kopyalanmamışsa hedef çalışma sayfasına başvurulup başvurulmayacağını belirtir. |
