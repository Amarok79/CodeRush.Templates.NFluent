# Introduction

This project provides a set of C#-based Code Templates for [CodeRush](https://www.devexpress.com/products/coderush/) targeted explicitly at writing unit tests with [NFluent](https://github.com/tpierrain/NFluent). For more information about CodeRush Code Templates refer to the official [CodeRush Documentation](https://docs.devexpress.com/CodeRushForRoslyn/115904/coding-assistance/code-templates).

Under Releases you can find XML files containing templates. These can be easily imported in CodeRush's [Template Configuration](https://docs.devexpress.com/CodeRushForRoslyn/115919/coding-assistance/code-templates/template-configuration).



# How to Use

For NFluent-style assertions, you typically start with template **kk** followed by Space which expands to:
    
    Check.That(<value>)

You can then enter the *value* to check, hit Enter, and then use one of the various templates from below, for example, **isf**, which expands to:

    Check.That(<value>)
        .IsFalse()

Enter the final semicolon, hit Enter again and done. Start again with **kk** for the next assertion.



# Templates

### General Templates

Template | Code
---------|-----------------------------------------------------
kk       | Check.That(*value*)
ise      |   .IsEqualTo(*expected*)
isne     |   .IsNotEqualTo(*expected*)
is0      |   .IsEqualTo(0)
is1      |   .IsEqualTo(1)
is2      |   .IsEqualTo(2)
isf      |   .IsFalse()
ist      |   .IsTrue()
isz      |   .IsEqualTo(0)
isn      |   .IsNull()
isnn     |   .IsNotNull()
isem     |   .IsEmpty()
isnem    |   .IsNotEmpty()
iss      |   .IsSameReferenceAs(*expected*)
isns     |   .Not.IsSameReferenceAs(*expected*)
idf      |   .IsDistinctFrom(*expected*)
iio      |   .IsInstanceOf\<*Type*>()
iiot     |   .IsInstanceOfType(*expected*)
inio     |   .IsNotInstanceOf\<*Type*>()
iniot    |   .IsNoInstanceOfType(*expected*)
ioo      |   .IsOneOf(*expected*)
hsf      |   .HasFieldsWithSameValues(*expected*)
hnsf     |   .HasNotFieldsWithSameValues(*expected*)


### Collection-specific Templates

Template | Code
---------|-----------------------------------------------------
con      |   .Contains(*expected*)
cone     |   .ContainsExactly(*expected*)
iomo     |   .IsOnlyMadeOf(*expected*)
ieqt     |   .IsEquivalentTo(*expected*)
hs       |   .HasSize(*expected*)
hfe      |   .HasFirstElement().Which
hle      |   .HasLastElement().Which
hea      |   .HasElementAt(*index*).Which


### String-specific Templates

Template | Code
---------|-----------------------------------------------------
isnoem   |   .IsNullOrEmpty()
isnows   |   .IsNullOrWhiteSpace()
iseic    |   .IsEqualIgnoringCase(*expected*)
stw      |   .StartsWith(*expected*)
enw      |   .EndsWith(*expected*)
mat      |   .Matches(*expected*)
matwc    |   .MatchesWildcards(*expected*)
ncon     |   .DoesNotContain(*expected*)
nmat     |   .DoesNotMatch(*expected*)


### Codeblock Templates

Template | Code
---------|-----------------------------------------------------
kkc      |   Check.ThatCode(() => *code-block*)
kkcc     |   Check.ThatCode(() => { *code-block* })
kkac     |   Check.ThatAsyncCode(async () => *code-block*)
kkacc    |   Check.ThatAsyncCode(async () => { *code-block* })
kkct     |   Check.ThatCode(() => *code-block*).Throws<*Exception*>();
kkact    |   Check.ThatAsyncCode(async () => *code-block*).Throws<*Exception*>();
