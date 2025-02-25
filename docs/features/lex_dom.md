# Feature: lex_dom <a name="start"></a>

Feature group | Feature type | Data type | Available for node types | Feature status
---  | --- | --- | --- | ---
[`Lexical`](featuresbygroup.md#lexical-features) | [`Node`](featuresbyfeaturetype.md#node-features) | [`string`](featuresbydatatype.md#string-datatype)  | [`word`](featuresbynodetype.md#word-nodes) | [✅](featuresbystatus.md#Trustworthy "Trustworthy") 

## Feature description

Lexical domain according to Semantic Dictionary of Biblical Greek (SDBG).

## Feature values

Value | Description | Frequency
--- | --- | ---
xxxyyy  | Lexical Domain value| 126757
'' | Empty | 11022

## Interpreting the data

Feature `lex_dom` is *to some extent* equivalent to a numerical representation of feature `[ln](ln.md#start)` and can be decoded using the following method. Take for example lex_domain = "089007". The 6-digit value "089007" first need to be split into two 3-digit parts: "087" and "007". The second part should be interpreted as a alphabetic (A=1, B=2, C=3, D=4, E=5, ..., Z=26). Taken the two parts together, this will result in 89G, which points to an entry in Louw-Nida. For this example (i.e. 89G) this maps to main section [relations](https://www.laparola.net/greco/louwnida.php?sezmag=89) and subsection [Cause and/or Reason](https://www.laparola.net/greco/louwnida.php?sezmag=89&sez1=15&sez2=38).

It is important to realize that the granularity of feature `lex_dom` is less than that of feature [`ln`](ln.md#start). Consider for example the ἀρχή in John 1:1. According to Louw-Nida Lexicon this can map to either a:beginning (aspect)=>68.1 or b:beginning (time)=>67.65. In Text-Fabric one value is attached to feature `lex_dom`, which is `067003`. Using the above explained method, this breaks down to "067" and "003" where the last part refers to section "C", which is actualy a range [(67.65-67.72)](https://www.laparola.net/greco/louwnida.php#67) within Louw Nida. 

## Note

See also related feature [ln](ln.md#start) (Louw-Nida lexical classification).

## Source description

Taken from XML attribute `domain` of tag `w` (word). The word sense data for this feature was compiled by the United Bible Societies MARBLE project. See [Macula-Greek Licence](https://github.com/Clear-Bible/macula-greek/blob/main/LICENSE.md).

---
###### *Browse all features by [node type](featuresbynodetype.md#start), [feature group](featuresbygroup.md#start), [data type](featuresbydatatype.md#start)  or [feature type](featuresbyfeaturetype.md#start).*
