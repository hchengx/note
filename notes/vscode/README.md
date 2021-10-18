VScode 使用与配置

## C/C++

### clangd

由于 clangd 依赖编译器前端提供索引和 AST 信息，这也注定了 clangd 在提供高准确跳转/补全的同时，也要用户配置好项目的“编译说明”，这个“编译说明”便被称为 [Compilation Database](https://clang.llvm.org/docs/JSONCompilationDatabase.html) 。

在 clangd 看来，Compilation Database 是一个名为 compile_commands.json 的 JSON 文件，它会记录每个 .c/.cpp 文件的编译依赖和编译选项。

[推荐配置](./settings/clangd.json)