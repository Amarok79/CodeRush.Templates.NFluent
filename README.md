# Introduction

\<TBD>


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


### Additional Collection-specific Templates

Template | Code
---------|-----------------------------------------------------
con      |   .Contains(*expected*)
hs       |   .HasSize(*expected*)


### Additional String-specific Templates

Template | Code
---------|-----------------------------------------------------
isnoem   |   .IsNullOrEmpty()
isnows   |   .IsNullOrWhiteSpace()
iseic    |   .IsEqualIgnoringCase(*expected*)
ssw      |   .StartsWith(*expected*)
sew      |   .EndsWith(*expected*)
sma      |   .Matches(*expected*)
smaw     |   .MatchesWildcards(*expected*)
ncon     |   .DoesNotContain(*expected*)
nsma     |   .DoesNotMatch(*expected*)




\<Work in Progress>

