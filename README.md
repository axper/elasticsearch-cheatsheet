# Elasticsearch Query DSL (Queries & Filters) Chatsheet

The angular brackets mean that the Filter/Query doesn't have a Query/Filter counterpart.

No angular brackets mean that both Filter/Query are available for this keyword.

## Meta
* `Exists`&lt;Filter&gt; - IS NOT NULL
* `Missing`&lt;Filter&gt; - IS NULL
* `Type`&lt;Filter&gt; - Document type
* `Ids` - 36-char document _uid
* `Indices` - Search in specified indices
* `Nested` - Search in nested documents
* `Has Child`
* `Has Parent`

## Wrapping/Combining
* `Bool` - combines other filters/queries` - must, must_not, should
* `Filtered`&lt;Query&gt; - Combines query with filter
* `Query` - Wraps any query, converts it to filter
* `And`&lt;Filter&gt;
* `Not`&lt;Filter&gt;
* `Or`&lt;Filter&gt;

## Search
* `Match All`
* `Range` - Number/Word range

### String search
* `Term` - Text contains the word
* `Terms` - Text contains multiple words
* `Match`&lt;Query&gt; - Text contains words
* `Prefix` - String prefix

#### Regex search
* `Regexp` - String regex
* `Wildcard`&lt;Query&gt; - Mini-regex

#### Fuzzy search
* `Fuzzy`&lt;Query&gt; - Text/Numbers similar/like to one specified
* `More Like This`&lt;Query&gt; - Find similar documents
