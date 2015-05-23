# Implementation of Autocompletion in Angular with a JavaScript-coded Trie

The Trie is written into a custom Angular directive that can be called
with <wdi-autocomplete></wdi-autocomplete>.  As is, this simply inserts
a text input with an Angular-generated list below that.  Currently, the
data is mocked in an Angular service called 'autoSearch' in the wordData
array, but the service could of course be reconfigured to pull wordData 
from any database source.  As is, being an Angular app, this solution
is backend agnostic.

# Twitter Typeahead

To create a dropdown interface for the Trie words, Twitter's jQuery Typeahead
solution could be dropped in from http://twitter.github.io/typeahead.js/examples/

# Installation

Running this app requires a server:

```
npm install -g http-server

http-server -a localhost -p 8080
```

Then, point your browser to:

```
localhost:8080
```

