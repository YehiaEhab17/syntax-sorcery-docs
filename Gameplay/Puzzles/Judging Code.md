

Code has to follow all the constraints first (check by AST? regex?)

checking time/memory complexity may be difficult? (piston returns cpu_time and memory, but that might depend on server load? could inject an operation counter into their code before sending it? could compare against different input sizes and see how the time grows? e.g. N=100, 1000, 10000?)

> self hosting might fix both of these?

cpu_time/memory would be accurate since its our server. on our own server we could have an API for AST matching for the languages we support? python/js have libraries for this. Java might have a parser. other languages (rust maybe?) need studying.

Could also store "optimal"/"intended" solution, and send both to piston, compare user solution with the benchmarks solution. e.g. 1.5x<= then it's better, 3x<= could be partial credit etc. as opposed to calculating thresholds manually, and thresholds may be affected by server load
