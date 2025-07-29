# sqlserver-mcp-scripts
Exemplo de uso do MCP do SQL Server com um server de banco de dados containerizado e consultado a dados de regiões do Brasil.

Arquivo mcp.json com configurações informados no Visual Studio Code:

```json
{
    "servers": {
        "mcp-sqlserver-testefinal": {
            "type": "stdio",
            "command": "C:\\DotNet8\\SQL-AI-samples-main\\SQL-AI-samples-main\\MssqlMcp\\dotnet\\MssqlMcp\\bin\\Debug\\net8.0\\MssqlMcp.exe",
            "args": [],
            "env": {
                "CONNECTION_STRING": "Server=localhost;Database=BaseDadosGeograficos;User Id=sa;Password=SqlServer2025!;TrustServerCertificate=True;"
            }
        }
    },
    "inputs": []
}
```

Exemplo de uso do MCP do SQL Server a partir do Visual Studio Code:

![MCP do SQL no VS Code](img/vscode-01.png)