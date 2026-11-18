---
title: "Validation Sınıfı"
linktitle: "Validation"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Validation sınıfı. Go'da validation'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/validation/
---

## Validation class

Veri doğrulama ayarlarını temsil eder.

```go

type Validation struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetOperator](./getoperator/) | Veri doğrulaması için operatörü temsil eder. |
| [SetOperator](./setoperator/) | Veri doğrulaması için operatörü temsil eder. |
| [GetAlertStyle](./getalertstyle/) | Doğrulama uyarı stilini temsil eder. |
| [SetAlertStyle](./setalertstyle/) | Doğrulama uyarı stilini temsil eder. |
| [GetType](./gettype/) | Veri doğrulama tipini temsil eder. |
| [SetType](./settype/) | Veri doğrulama tipini temsil eder. |
| [GetInputMessage](./getinputmessage/) | Veri doğrulama giriş mesajını temsil eder. |
| [SetInputMessage](./setinputmessage/) | Veri doğrulama giriş mesajını temsil eder. |
| [GetInputTitle](./getinputtitle/) | Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder. |
| [SetInputTitle](./setinputtitle/) | Veri-doğrulama giriş iletişim kutusunun başlığını temsil eder. |
| [GetErrorMessage](./geterrormessage/) | Veri doğrulama hata mesajını temsil eder. |
| [SetErrorMessage](./seterrormessage/) | Veri doğrulama hata mesajını temsil eder. |
| [GetErrorTitle](./geterrortitle/) | Veri-doğrulama hata iletişim kutusunun başlığını temsil eder. |
| [SetErrorTitle](./seterrortitle/) | Veri-doğrulama hata iletişim kutusunun başlığını temsil eder. |
| [GetShowInput](./getshowinput/) | Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir. |
| [SetShowInput](./setshowinput/) | Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir. |
| [GetShowError](./getshowerror/) | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir. |
| [SetShowError](./setshowerror/) | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir. |
| [GetIgnoreBlank](./getignoreblank/) | Aralık veri doğrulaması tarafından boş değerlerin izin verilip verilmeyeceğini belirtir. |
| [SetIgnoreBlank](./setignoreblank/) | Aralık veri doğrulaması tarafından boş değerlerin izin verilip verilmeyeceğini belirtir. |
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Belirli hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Belirli hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar. |
| [GetFormula1](./getformula1/) | Veri doğrulaması ile ilişkili değeri veya ifadeyi temsil eder. |
| [SetFormula1_String](./setformula1_string/) | Veri doğrulaması ile ilişkili değeri veya ifadeyi temsil eder. |
| [GetFormula2](./getformula2/) | Veri doğrulaması ile ilişkili değeri veya ifadeyi temsil eder. |
| [SetFormula2_String](./setformula2_string/) | Veri doğrulaması ile ilişkili değeri veya ifadeyi temsil eder. |
| [GetListValue](./getlistvalue/) | Belirtilen hücre için doğrulama listesinin değerini al. |
| [GetValue1](./getvalue1/) | Veri doğrulaması ile ilişkili ilk değeri temsil eder. |
| [SetValue1](./setvalue1/) | Veri doğrulaması ile ilişkili ilk değeri temsil eder. |
| [GetValue2](./getvalue2/) | Veri doğrulaması ile ilişkili ikinci değeri temsil eder. |
| [SetValue2](./setvalue2/) | Veri doğrulaması ile ilişkili ikinci değeri temsil eder. |
| [GetValue](./getvalue/) | Belirli hücredeki doğrulamanın değerini al. |
| [GetInCellDropDown](./getincelldropdown/) | Veri doğrulamasının kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir. |
| [SetInCellDropDown](./setincelldropdown/) | Veri doğrulamasının kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir. |
| [GetAreas](./getareas/) | Veri doğrulama ayarlarını içeren tüm CellArea'ları alır. |
| [AddArea_CellArea](./addarea_cellarea/) | Doğrulamayı alana uygular. |
| [AddArea_CellArea_Bool_Bool](./addarea_cellarea_bool_bool/) | Doğrulamayı alana uygular. |
| [AddAreas](./addareas/) | Doğrulamayı verilen alanlara uygular. |
| [RemoveArea](./removearea/) | Aralıktaki doğrulama ayarlarını kaldır. |
| [RemoveAreas](./removeareas/) | Bu doğrulamayı verilen alanlardan kaldırır. |
| [RemoveACell](./removeacell/) | Hücredeki doğrulama ayarlarını kaldır. |
| [Copy](./copy/) | Doğrulamayı kopyala. |
