## Android分屏模式

Android7.0（API24）新增对同时显示多个应用的支持。在手持设备上，两个应用可以在分屏模式中左右并排或者上下并排显示。在电视设备上，应用可以使用画中画模式，在用户与另一个交互的同时继续播放视频。

从Android8.0开始，应用可以将自身置于画中画模式，从而使其能在用户浏览其他应用或与之交互时继续显示内容。

多窗口模式不会更改Activity生命周期。

在多窗口模式中，只有最近在指定时间内与用户交互的 Activity 为活动状态。此 Activity 被视为*顶端* Activity，而且是唯一处于 [`RESUMED`](https://developer.android.com/reference/androidx/lifecycle/Lifecycle.State.html?hl=zh-cn) 状态的 Activity。其他所有可见的Activity均处于`started`而非resume。但是这些处于可见而且非恢复状态

