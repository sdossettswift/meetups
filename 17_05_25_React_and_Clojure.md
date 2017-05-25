# houston.js
## clojure script x react
- Chris Oakman
- sponsored by Toptal (Ethan - North American Community Global Lead)

# intro to clojurescript
- clojure complied to js
	- clojure typically compiles to java
- functional language - 
 - no state. things change b/c of functions, not b/c of state or mutation
 - js can be functional... but is not functional 
- dynamically typed
- lisp syntax 
- language != runtime, although they are often

## why clojure?
- simple, practical 
- stable, flexible syntax (future proof)
 - instead of re-writing source code, features are just added as new libraries 
 - no wierd conventions *looking at you, js* 
- powerful core library
- persistent data structures as default
- awesome community  (smart && nice)
- great video on clojure: **Simple Made Easy** - Rich Hickey  [https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/SimpleMadeEasy.md]
- ** wtf is a monad? **

### why clojurescript?
- language level state mgmt
- build system is part of the lang
- leverages the best of google closure toolchain
- flexible syntax: HTML, async, React
- stable 
- great video on cljs: ClojureScript for Skeptics - Derek Slager

# intro to react.js
- declarative DOM -- DOM as a function of data
- library handles DOM transition
- component-based
- small, functional interface
- vDOM
- [insert diagram here]
- tree of data - lisp syntax
- under the hood, react has a very small functional interface
- components are not megacomplex

# why cl.js x react.js
- flexible syntax (no JSX!!)
- immutable data by default
- components/functions compose naturally
- no one is using vDOM setup w/out JSX but JSX is madness 
- should component update w/ immutable data is a gut check
- persistent data structure 
- sharing structure - d &&  d' both point to b -- the check happens instantaneously 
  


# demo



