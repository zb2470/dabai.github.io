### 3. 系统权限表的滞后或缺失
在某些 MLflow 版本或特定配置下，`NO_PERMISSIONS` 模式下创建对象时，插件可能没有自动将创建者设为“拥有者”。

*   **检查方法**：查询 Auth 数据库（你在上一个问题中提到的那个库）中的 `registered_models_permissions` 表。
*   **预期结果**：应该有一行记录显示该 `user_id` 对该 `name` (模型名) 拥有 `MANAGE` 权限。如果没有，手动添加。
