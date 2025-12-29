*   **可以不同吗？** 可以。
*   **怎么做？** 在 `database_uri` 后面加上 `?options=-csearch_path=你的Schema名`。
*   **注意点**：必须确保数据库中该 Schema 已预先存在，且连接用户拥有该 Schema 的 `CREATE` 和 `USAGE` 权限。
