# Tasks — Week 01: JavaScript Core

Task IDs and acceptance criteria are stable. **No ready-made solutions**. Use plain JavaScript without external libraries unless explicitly allowed. Provide self-written examples/tests.

## Day 1: types and coercion
### JS-002 — Predict JS results
Before running code, predict the **value and type** of: `typeof null`, `[] == false`, `0 == '0'`, `0 === '0'`, `Boolean('false')`, `typeof NaN`, `['1','2'] + 3`, `({a:1} === {a:1})`. Verify afterward and explain differences.
**Accept:** 8 explanations; at least 6 correct predictions before running; explain any corrections.

## Day 2: closures
### JS-001 — createCounter(initialValue)
Return an object with `increment()`, `decrement()`, `getValue()`. Example: from 5, increment -> 6, increment -> 7, decrement -> 6, getValue -> 6.
**Constraints:** No global mutable state, classes or localStorage. State cannot be overwritten directly through returned object properties. Instances are independent.
**Accept:** starts at 0 and -3, alternating calls, two independent counters, inaccessible internal state.

### JS-003 — once(fn)
Wrap `fn` so only its first invocation runs it; all later calls return the cached first result. Preserve original arguments and `this`.
**Accept:** side effect runs once, subsequent return consistent, `this`/arguments preserved; document behavior if original function throws.

## Day 3: arrays and objects
### JS-004 — myMap and myFilter
Implement `myMap(array, callback)`, `myFilter(array, callback)` without native map/filter. Callback receives (element,index,array). Input unchanged.
**Accept:** empty array, index use, falsey values, no input mutation. Sparse arrays may be out of scope if documented.

### JS-005 — groupBy(items,key)
Group objects by stringified property value; e.g. `[{type:'a',id:1},{type:'b',id:2},{type:'a',id:3}]` grouped by `type`.
**Accept:** empty, multiple groups, preserve order, no input mutation, document missing keys, prevent `__proto__` key bugs.

## Day 4: async/event loop
### JS-006 — Event loop reasoning
Predict output and explain stack / microtasks / tasks:
```js
console.log('A');
setTimeout(() => console.log('B'), 0);
Promise.resolve().then(() => console.log('C'));
queueMicrotask(() => console.log('D'));
console.log('E');
```
**Accept:** exact ordering with explanation, zero-timeout not synchronous.

### JS-007 — retry(fn, attempts)
Implement `async retry(fn,attempts)` until async function resolves or attempts run out; attempts includes first call, must be a positive integer, final rejection retains last error, no delay required.
**Accept:** first success, third success, persistent failure, invalid attempts, exact number of calls.

## Days 5–6: mini-project
### JS-008 — Searchable Directory
Responsive HTML/CSS/JS app with >=20 local records `{id,name,role,city}`. Search names case-insensitively; filter roles; sort A–Z/Z–A; visible result count; empty state; 300 ms debounced search; persist sort preference in localStorage.
**Constraints:** No framework or prebuilt search/sort libraries. All controls keyboard accessible; don't inject raw record HTML.
**Accept:** behaviors above, mobile from 320px, five documented test scenarios, readable structure.

## Day 7: checkpoint
### JS-009 — Week 1 mock
20 questions across types/scope/closures/arrays/async, two unseen 20-minute coding questions, five-minute explanation of JS-008.
**Accept:** record evidence, strengths, gaps and scores in PROGRESS.md; no automatic pass.

## Future placeholder IDs
TS-001+ (week 4); REACT-001+ (weeks 5–6); TEST-001+ (week 7); PERF-001+ (week 8); DESIGN-001+ (week 9); BACKEND-001+ (week 10); INT-001+ (weeks 11–12). Add specifics only when scheduled.