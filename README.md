# AndroidFoundationCompoent
The project includes the needs of the basic components required by Android application developers。

## 1.Asynchronous sequential task queue 异步顺序任务队列
可以异步执行的，带顺序的任务队列
### 1.1 可以顺序执行任务
顺序执行任务 A B C，如果 A 没有执行成功，B 会等待 A 执行成功之后再执行，C 会等待 B 执行成功之后再执行。
### 1.2 可以随意切换任务执行线程
A B C 可以在不同的线程中执行，也可以在同一个线程中执行。
### 1.3 可以方便进行任务重复调用
A 执行失败，可以发起 A 任务重试，也会自动重试 B C 任务。
### 1.4 可以随意增加后续任务数量
可以在任何时刻随意在 A B C 队列中增加 C D E F 等顺序执行的任务。
