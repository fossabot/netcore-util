# UtilExt Class
**Namespace:** SearchAThing

**Inheritance:** Object → UtilExt

(No Description)

## Signature
```csharp
public static class UtilExt
```
## Methods
|**Name**|**Summary**|
|---|---|
|[Assign](UtilExt/Assign.md) (static)|assign public properties of src to dst object|
|[CompareTol](UtilExt/CompareTol.md) (static)||
|[ContainsIgnoreCase](UtilExt/ContainsIgnoreCase.md) (static)|check if given string contains the part ( ignoring case )|
|[CopyFrom](UtilExt/CopyFrom.md) (static)|copy properties from other object ; if match functor specified it copies only matched properties|
|[CopyFromExclude](UtilExt/CopyFromExclude.md) (static)||
|[CopyFromInclude](UtilExt/CopyFromInclude.md) (static)||
|[Details](UtilExt/Details.md) (static)||
|[DetailsObject](UtilExt/DetailsObject.md) (static)||
|[Equals](UtilExt/Equals.md)||
|[EqualsAutoTol](UtilExt/EqualsAutoTol.md) (static)|Returns true if two numbers are equals using a default tolerance of 1e-6 about the smaller one.|
|[EqualsTol](UtilExt/EqualsTol.md) (static)||
|[Export](UtilExt/Export.md) (static)|export to a string ( invariant ) comma separated|
|[GetHashCode](UtilExt/GetHashCode.md)||
|[GetJsonArray](UtilExt/GetJsonArray.md) (static)|return dynamic array from given [[xx],[yy],...] json array|
|[GetType](UtilExt/GetType.md)||
|[GreatThanOrEqualsTol](UtilExt/GreatThanOrEqualsTol.md) (static)||
|[GreatThanTol](UtilExt/GreatThanTol.md) (static)||
|[HumanReadable](UtilExt/HumanReadable.md) (static)|Returns a human readable bytes length. (eg. 1000, 1K, 1M, 1G, 1T)<br/>            if onlyBytesUnit is set to false it will enable representation through K, M, G, T suffixes|
|[Import](UtilExt/Import.md) (static)|parse given array of doubles ( invariant ) comma separated|
|[InvariantDate](UtilExt/InvariantDate.md) (static)|return yyyy-MM-dd representation|
|[InvarianteDateTime](UtilExt/InvarianteDateTime.md) (static)|return yyyy-MM-dd HH:mm.ss representation|
|[InvariantTime](UtilExt/InvariantTime.md) (static)|return HH:mm.ss representation|
|[InvDoubleParse](UtilExt/InvDoubleParse.md) (static)|Invariant culture double parse|
|[IsInRange](UtilExt/IsInRange.md) (static)|eval if a number fits in given range<br/>            eg.<br/>            - "[0, 10)" are numbers from 0 (included) to 10 (excluded)<br/>            - "[10, 20]" are numbers from 10 (included) to 20 (included)<br/>            - "(30,)" are numbers from 30 (excluded) to +infinity|
|[Latest](UtilExt/Latest.md) (static)|convert a string that exceed N given characters length to {prefix}{latest N chars}|
|[LessThanOrEqualsTol](UtilExt/LessThanOrEqualsTol.md) (static)||
|[LessThanTol](UtilExt/LessThanTol.md) (static)||
|[Lines](UtilExt/Lines.md) (static)|Smart line splitter that split a text into lines whatever unix or windows line ending style.<br/>            By default its remove empty lines.|
|[Magnitude](UtilExt/Magnitude.md) (static)|Magnitude of given number. (eg. 190 -> 1.9e2 -> 2)<br/>            (eg. 0.0034 -> 3.4e-3 -> -3)|
|[MatchesFilter](UtilExt/MatchesFilter.md) (static)|Checks whatever fields matches given filter all words in any of inputs.<br/>            ex. fields={ "abc", "de" } filter="a" results: true<br/>            ex. fields={ "abc", "de" } filter="a d" results: true<br/>            ex. fields={ "abc", "de" } filter="a f" results: false<br/>            autoskips null fields check;<br/>            returns true if filter empty|
|[Mean](UtilExt/Mean.md) (static)|Mean of given numbers|
|[MRound](UtilExt/MRound.md) (static)|Round the given value using the multiple basis|
|[MRound](UtilExt/MRound.md#mroundnullabledouble-double) (static)|Round the given value using the multiple basis<br/>            if null return null|
|[MRound](UtilExt/MRound.md#mrounddouble-nullabledouble) (static)|Round the given value using the multiple basis|
|[NextLine](UtilExt/NextLine.md) (static)||
|[NormalizeFilename](UtilExt/NormalizeFilename.md) (static)||
|[NormalizeWorksheetName](UtilExt/NormalizeWorksheetName.md) (static)|convert invalid worksheet characters :\/?*[]' into underscore|
|[ParseInt](UtilExt/ParseInt.md) (static)||
|[PrecisionDifference](UtilExt/PrecisionDifference.md) (static)|Compute precision difference between two numbers<br/>            so that results will be a positive number >= 0<br/>            that measures how much they equals.<br/>            For example a result of 1e-6 states that two given numbers are equals until 6 precision digits.<br/>            111111111111111d.PrecisionDifference(111111011111111d) == 1.000000000139778E-06<br/>            <br/>            The function useful to states if two computation results equals except for some precision digits.<br/>            <br/>            Other examples:<br/>            111111111111111d.PrecisionDifference(111111111111111d) == 0<br/>            111111111111111d.PrecisionDifference(191111111111111d) == 0.8<br/>            111111111111111d.PrecisionDifference(111111111111119d) == 7.9936057773011271E-14<br/>            1.23e-210.PrecisionDifference(1.23001e-210) == 9.9999999998434674E-06<br/>            21.23e-210.PrecisionDifference(1.23001e-210) == 10.892990000000001|
|[RegexMatch](UtilExt/RegexMatch.md) (static)|retrieve nr. of occurrence of given pattern through regex|
|[Repeat](UtilExt/Repeat.md) (static)|Repeat given string for cnt by concatenate itself|
|[Sign](UtilExt/Sign.md) (static)|returns 1.0 if n>=0<br/>            -1 otherwise|
|[Sign](UtilExt/Sign.md#signdouble) (static)|returns 1.0 if n>=0<br/>            -1 otherwise|
|[SmartDoubleParse](UtilExt/SmartDoubleParse.md) (static)|parse string that represent number without knowing current culture<br/>            so that it can parse "1.2" or "1,2" equivalent to 1.2<br/>            it will throw error more than one dot or comma found|
|[Sort](UtilExt/Sort.md) (static)|sort obc|
|[Split](UtilExt/Split.md) (static)|split string with given separator string|
|[Stringify](UtilExt/Stringify.md) (static)||
|[StripBegin](UtilExt/StripBegin.md) (static)|Returns the given string stripped from the given part if exists at beginning.|
|[StripBegin](UtilExt/StripBegin.md#stripbeginstring-string-bool) (static)|Returns the given string stripped from the given part if exists at beginning.|
|[StripEnd](UtilExt/StripEnd.md) (static)|Returns the given string stripped from the given part if exists at end.|
|[StripEnd](UtilExt/StripEnd.md#stripendstring-string-bool) (static)|Returns the given string stripped from the given part if exists at end.|
|[ToDeg](UtilExt/ToDeg.md) (static)|convert given angle(rad) to degree|
|[ToExpando](UtilExt/ToExpando.md) (static)|create an expando object by copying given src|
|[ToJson](UtilExt/ToJson.md) (static)||
|[ToRad](UtilExt/ToRad.md) (static)|convert given angle(grad) to radians|
|[ToString](UtilExt/ToString.md)||
|[ToString](UtilExt/ToString.md#tostringdouble-int) (static)|format number so that show given significant digits. (eg. 2.03 with significantDigits=4 create "2.0300")|
|[ToStringWrapper](UtilExt/ToStringWrapper.md) (static)||
|[TrimNonNumericCharacters](UtilExt/TrimNonNumericCharacters.md) (static)|removes all characters that aren't 0-9 dot or comma|
|[UnspecifiedAsUTCDateTime](UtilExt/UnspecifiedAsUTCDateTime.md) (static)|if given dt has unspecified kind rectifies to UTC without any conversion|
|[WildcardMatch](UtilExt/WildcardMatch.md) (static)|return true if given string matches the given pattern<br/>            the asterisk '*' character replace any group of chars<br/>            the question '?' character replace any single character|
|[WildcardToRegex](UtilExt/WildcardToRegex.md) (static)|convert wildcard pattern to regex<br/>            the asterisk '*' character replace any group of chars<br/>            the question '?' character replace any single character|
|[WithIndex](UtilExt/WithIndex.md) (static)|enumerable extension to enumerate itself into an (item, idx) set|
|[WithIndexIsLast](UtilExt/WithIndexIsLast.md) (static)|enumerable extension to enumerate itself into an (item, idx, isLast) set|
## Conversions
