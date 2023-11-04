1. API.csproj
調整 <Nullable>disable</Nullable>，此處設定為 Nullable 之後 class 就不會有底線警告。
- enable：表示未明確標記為可空就一定要有值。
- disable：不管是有值或 null 都接受。

2. prop 指令快速建立 class 項目。

3.  Linq --> DbSet --> SQL --> Database
- Linq：var products = context.products.ToList()
- SQL：select * from Products

4. 使用 "dotnet new gitignore" 看哪些避免上傳到 git

5. entity framwork 安裝流程
- dotnet tool install --global dotnet-ef --version 7.0.2
- dotnet tool list -g 列出安裝的名稱與版本
- dotnet tool update --global dotnet-ef 更新到最新版本
- dotnet ef entity framework 安裝成功會看到一隻獨角獸
- dotnet ef migrations add instialcreate -o Data/Migrations
Build started...
Build succeeded.
Done. To undo this action, use 'ef migrations remove'
