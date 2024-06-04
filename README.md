# 專案設定與指令

## 1. API.csproj
調整 `<Nullable>disable</Nullable>`，此處設定為 Nullable 之後 class 就不會有底線警告。
- enable：表示未明確標記為可空就一定要有值。
- disable：不管是有值或 null 都接受。

## 2. prop 指令快速建立 class 項目

## 3. Linq --> DbSet --> SQL --> Database
- Linq：`var products = context.products.ToList()`
- SQL：`SELECT * FROM Products`

## 4. 使用 "dotnet new gitignore" 查看哪些檔案應避免上傳到 git

## 5. Entity Framework 安裝流程
- 安裝 Entity Framework 工具：  
  ```bash
  dotnet tool install --global dotnet-ef --version 7.0.2

- 列出已安裝的工具名稱與版本：
  ```bash
  dotnet tool list -g

- 更新到最新版本：
  ```bash
  dotnet tool update --global dotnet-ef

- 安裝成功會看到一隻獨角獸：
  ```bash
  dotnet ef

- 添加初始遷移：
  ```bash
  dotnet ef migrations add initialcreate -o Data/Migrations

- 輸出：
  ```bash
  Build started...
  Build succeeded.
  Done. To undo this action, use 'ef migrations remove'

- 更新資料庫：
  ```bash
  dotnet ef database update
