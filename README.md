# sqlserver-mcp-scripts
Exemplo de uso do MCP do SQL Server com um server de banco de dados containerizado e consultado a dados de regiões do Brasil. Inclui Docker Compose para criação do ambiente de testes.

Um pouco mais sobre o MCP Server do SQL Server:
- [**Anúncio no blog oficial**](https://devblogs.microsoft.com/azure-sql/introducing-mssql-mcp-server/)
- [**Instruções de uso da versão criada em .NET 8**](https://github.com/Azure-Samples/SQL-AI-samples/blob/main/MssqlMcp/dotnet/README.md)

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
![Aplicação em execução](img/vscode-01.png)
