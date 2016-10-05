index:
type: 'List of Strings',
default: [''],
definition: 'A comma-separated list of index names to search; use `_all`
or empty string to perform the operation on all indices'

doc_type:
type: 'List of Strings',
default: [''],
definition: 'A comma-separated list of document types to search; leave
empty to perform the operation on all types'

body:
type: 'String',
default: '',
definition: 'The search definition using the Query DSL'



:arg _source: True or false to return the _source field or not, or a
list of fields to return

:arg _source_exclude: A list of fields to exclude from the returned
_source field

:arg _source_include: A list of fields to extract and return from the
_source field
:arg allow_no_indices: Whether to ignore if a wildcard indices
expression resolves into no concrete indices. (This includes `_all`
 string or when no indices have been specified)
 :arg analyze_wildcard: Specify whether wildcard and prefix queries
 should be analyzed (default: false)
 :arg analyzer: The analyzer to use for the query string
 :arg default_operator: The default operator for query string query (AND
  or OR), default 'OR', valid choices are: 'AND', 'OR'
  :arg df: The field to use as default where no field prefix is given in
  the query string
  :arg expand_wildcards: Whether to expand wildcard expression to concrete
  indices that are open, closed or both., default 'open', valid
  choices are: 'open', 'closed', 'none', 'all'
  :arg explain: Specify whether to return detailed information about score
  computation as part of a hit
  :arg fielddata_fields: A comma-separated list of fields to return as the
  field data representation of a field for each hit
  :arg fields: A comma-separated list of fields to return as part of a hit
  :arg from\_: Starting offset (default: 0)
  :arg ignore_unavailable: Whether specified concrete indices should be
  ignored when unavailable (missing or closed)
  :arg lenient: Specify whether format-based query failures (such as
   providing text to a numeric field) should be ignored
   :arg lowercase_expanded_terms: Specify whether query terms should be
   lowercased
   :arg preference: Specify the node or shard the operation should be
   performed on (default: random)
   :arg q: Query in the Lucene query string syntax
   :arg request_cache: Specify if request cache should be used for this
   request or not, defaults to index level setting
   :arg routing: A comma-separated list of specific routing values
   :arg scroll: Specify how long a consistent view of the index should be
   maintained for scrolled search
   :arg search_type: Search operation type, valid choices are:
   'query_then_fetch', 'dfs_query_then_fetch', 'count', 'scan'
   :arg size: Number of hits to return (default: 10)
   :arg sort: A comma-separated list of <field>:<direction> pairs
   :arg stats: Specific 'tag' of the request for logging and statistical
   purposes
   :arg suggest_field: Specify which field to use for suggestions
   :arg suggest_mode: Specify suggest mode, default 'missing', valid
   choices are: 'missing', 'popular', 'always'
   :arg suggest_size: How many suggestions to return in response
   :arg suggest_text: The source text for which the suggestions should be
   returned
   :arg terminate_after: The maximum number of documents to collect for
   each shard, upon reaching which the query execution will terminate
   early.
   :arg timeout: Explicit operation timeout
   :arg track_scores: Whether to calculate and return scores even if they
   are not used for sorting
   :arg version: Specify whether to return document version as part of a
   hit
