## Meta
* `And`<Filter>
* `Not`<Filter>
* `Or`<Filter>
* `Exists`<Filter> - IS NOT NULL
* `Missing`<Filter> - IS NULL
* `Type`<Filter> - Document type
* `Ids` - 36-char document _uid
* `Indices` - Search in specified indices
* `Nested` - Search in nested documents
* `Has Child`
* `Has Parent`

## Wrapping/Combining
* `Bool` - combines other filters/queries` - must, must_not, should
* `Filtered`<Query> - Combines query with filter
* `Query` - Wraps any query, converts it to filter

## Search
* `Match All`
* `Range` - Number/Word range

## String search
* `Term` - Text contains the word
* `Terms` - Text contains multiple words
* `Match`<Query> - Text contains words
* `Prefix` - String prefix

#### Regex search
* `Regexp` - String regex
* `Wildcard`<Query> - Mini-regex

#### Fuzzy search
* `Fuzzy`<Query> - Text/Numbers similar/like to one specified
* `More Like This`<Query> - Find similar documents
