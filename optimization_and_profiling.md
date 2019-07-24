## Optimization

 - profiling = "Strategy for optimizing code intelligently"

### CPython vs PyPy

 - PyPy performs a profiler-driven optimization (JIT compiler). What PyPy is doing is hard and it is not a magic wand, we still need to optimize our code.

### Why not optimize everything ?

 - Fast code is expensive

 - Optimized code is harder to maintain

   - Harder to reason

   - What you wrote is not what you run

 - "Premature optimization is the root of all evil". Only 3% of the code needs to be optimized.

### Optimization Workflow

 - Find problematic regions (functions)

 - Find problematic lines

 - See what is the problem

 - Solve it

 - Check if problem is solve

#### Advices

 - Scripted Tests

 - Keep your profiles while you optimize

 - Commit frequently with verbose messages (did this, improved this much etc.) and consider to revert if something goes badly.

### Different Profiling Levels

 - `time`

 - `timeit`

 - `cProfile`

 - `line_profiler`