##TextAutonumberScheme Enum
'TextAutonumberScheme enum. Encapsulates the object that represents textautonumberscheme in Go.'
## TextAutonumberScheme Enum
Represents all automatic number scheme.
```go
type TextAutonumberScheme int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) |  |
|[AlphaLcParenBoth](./alphalcparenboth/) | (a), (b), (c), … |
|[AlphaLcParenR](./alphalcparenr/) | a), b), c), … |
|[AlphaLcPeriod](./alphalcperiod/) | a., b., c., … |
|[AlphaUcParenBoth](./alphaucparenboth/) | (A), (B), (C), … |
|[AlphaUcParenR](./alphaucparenr/) | A), B), C), … |
|[AlphaUcPeriod](./alphaucperiod/) | A., B., C., … |
|[Arabic1Minus](./arabic1minus/) | Bidi Arabic 1 (AraAlpha) with ANSI minus symbol |
|[Arabic2Minus](./arabic2minus/) | Bidi Arabic 2 (AraAbjad) with ANSI minus symbol |
|[ArabicDbPeriod](./arabicdbperiod/) | Dbl-byte Arabic numbers w/ double-byte period |
|[ArabicDbPlain](./arabicdbplain/) | Dbl-byte Arabic numbers |
|[ArabicParenBoth](./arabicparenboth/) | (1), (2), (3), … |
|[ArabicParenR](./arabicparenr/) | 1), 2), 3), … |
|[ArabicPeriod](./arabicperiod/) | 1., 2., 3., … |
|[ArabicPlain](./arabicplain/) | 1, 2, 3, … |
|[CircleNumDbPlain](./circlenumdbplain/) | Dbl-byte circle numbers (1-10 circle[0x2460-], 11-arabic numbers) |
|[CircleNumWdBlackPlain](./circlenumwdblackplain/) | Wingdings black circle numbers |
|[CircleNumWdWhitePlain](./circlenumwdwhiteplain/) | Wingdings white circle numbers (0-10 circle[0x0080-],11- arabic numbers) |
|[Ea1ChsPeriod](./ea1chsperiod/) | EA: Simplified Chinese w/ single-byte period |
|[Ea1ChsPlain](./ea1chsplain/) | EA: Simplified Chinese (TypeA 1-99, TypeC 100-) |
|[Ea1ChtPeriod](./ea1chtperiod/) | EA: Traditional Chinese w/ single-byte period |
|[Ea1ChtPlain](./ea1chtplain/) | EA: Traditional Chinese (TypeA 1-19, TypeC 20-) |
|[Ea1JpnChsDbPeriod](./ea1jpnchsdbperiod/) | EA: Japanese w/ double-byte period |
|[Ea1JpnKorPeriod](./ea1jpnkorperiod/) | EA: Japanese/Korean w/ single-byte period |
|[Ea1JpnKorPlain](./ea1jpnkorplain/) | EA: Japanese/Korean (TypeC 1-) |
|[Hebrew2Minus](./hebrew2minus/) | Bidi Hebrew 2 with ANSI minus symbol |
|[HindiAlpha1Period](./hindialpha1period/) | Hindi alphabet period - consonants |
|[HindiAlphaPeriod](./hindialphaperiod/) | Hindi alphabet period - vowels |
|[HindiNumParenR](./hindinumparenr/) | Hindi numerical parentheses - right |
|[HindiNumPeriod](./hindinumperiod/) | Hindi numerical period |
|[RomanLcParenBoth](./romanlcparenboth/) | (i), (ii), (iii), … |
|[RomanLcParenR](./romanlcparenr/) | i), ii), iii), … |
|[RomanLcPeriod](./romanlcperiod/) | i., ii., iii., … |
|[RomanUcParenBoth](./romanucparenboth/) | (I), (II), (III), … |
|[RomanUcParenR](./romanucparenr/) | I), II), III), … |
|[RomanUcPeriod](./romanucperiod/) | I., II., III., … |
|[ThaiAlphaParenBoth](./thaialphaparenboth/) | Thai alphabet parentheses - both |
|[ThaiAlphaParenR](./thaialphaparenr/) | Thai alphabet parentheses - right |
|[ThaiAlphaPeriod](./thaialphaperiod/) | Thai alphabet period |
|[ThaiNumParenBoth](./thainumparenboth/) | Thai numerical parentheses - both |
|[ThaiNumParenR](./thainumparenr/) | Thai numerical parentheses - right |
|[ThaiNumPeriod](./thainumperiod/) | Thai numerical period |
