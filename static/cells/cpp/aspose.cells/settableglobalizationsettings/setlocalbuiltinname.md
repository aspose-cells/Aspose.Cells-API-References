##Aspose::Cells::SettableGlobalizationSettings::SetLocalBuiltInName method
'Aspose::Cells::SettableGlobalizationSettings::SetLocalBuiltInName method. Sets the locale dependent text for the built-in name with given standard name text in C++.'
## SettableGlobalizationSettings::SetLocalBuiltInName(const U16String\&, const U16String\&, bool) method
Sets the locale dependent text for the built-in name with given standard name text.
```cpp
void Aspose::Cells::SettableGlobalizationSettings::SetLocalBuiltInName(const U16String &standardName, const U16String &localName, bool bidirectional)
```
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | const U16String\& | Standard(en-US locale) name text of built-in name. |
| localName | const U16String\& | Locale dependent name text |
| bidirectional | bool | Whether map the local name text to standard name text automatically. If true, the local name text will be mapped to standard name text automatically so user does not need to call SetStandardBuiltInName(string, string, bool) again for the same standard and local names pair |
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [SettableGlobalizationSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## SettableGlobalizationSettings::SetLocalBuiltInName(const char16_t*, const char16_t*, bool) method
Sets the locale dependent text for the built-in name with given standard name text.
```cpp
void Aspose::Cells::SettableGlobalizationSettings::SetLocalBuiltInName(const char16_t *standardName, const char16_t *localName, bool bidirectional)
```
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | const char16_t* | Standard(en-US locale) name text of built-in name. |
| localName | const char16_t* | Locale dependent name text |
| bidirectional | bool | Whether map the local name text to standard name text automatically. If true, the local name text will be mapped to standard name text automatically so user does not need to call SetStandardBuiltInName(string, string, bool) again for the same standard and local names pair |
## See Also
* Class [Vector](../../vector/)
* Class [SettableGlobalizationSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
