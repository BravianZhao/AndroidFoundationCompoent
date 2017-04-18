# AndroidFoundationCompoent
The project includes the needs of the basic components required by Android application developers。

## 1.Asynchronous sequential task queue 异步顺序任务队列
可以异步执行的，带顺序的任务队列，比如现在需要顺序执行任务 A B C，如果 A 没有执行成功，B 会等待 A 执行成功之后再执行，C 会等待 B 执行成功之后再执行。A B C 可以在不同的线程中执行，也可以在同一个线程中执行。
