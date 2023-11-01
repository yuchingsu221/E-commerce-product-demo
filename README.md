1. API.csproj
調整 <Nullable>disable</Nullable>，此處設定為 Nullable 之後 class 就不會有底線警告。
- enable：表示未明確標記為可空就一定要有值。
- disable：不管是有值或 null 都接受。

2. prop 指令快速建立 class 項目。

3.  Linq --> DbSet --> SQL --> Database
- Linq：var products = context.products.ToList()
- SQL：select * from Products

4. 使用 "dotnet new gitignore" 看哪些避免上傳到 git