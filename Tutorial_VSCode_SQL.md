# 🛠️ Tutorial: Configuração do VS Code para SQL Server (mssql)

Este tutorial documenta o processo de transformação do Visual Studio Code em um ambiente de desenvolvimento integrado (IDE) para o **Microsoft SQL Server**.

## 📝 Introdução Técnica
A extensão **mssql** para Visual Studio Code é um suplemento desenvolvido pela Microsoft que permite a conexão com instâncias do SQL Server (locais ou na nuvem). Ela oferece recursos de:
*   **IntelliSense:** Autocompletar inteligente para palavras-chave de T-SQL e esquemas de banco de dados.
*   **Query Execution:** Execução de scripts diretamente no editor com visualização de resultados em grade.
*   **Gestão de Conexões:** Armazenamento de perfis de conexão para acesso rápido a diferentes bancos de dados.

---

## 🚀 Passo a Passo de Configuração

### 1. Instalação da Extensão
1. Abra o **VS Code**.
2. Vá até o menu de **Extensões** (`Ctrl + Shift + X`).
3. Pesquise por `SQL Server (mssql)` e clique em **Install**.

### 2. Criando uma Conexão
1. No menu lateral esquerdo, clique no ícone do **SQL Server**.
2. Clique no ícone de **+ (Add Connection)**.
3. Insira as seguintes informações quando solicitado:
   * **Server Name:** `localhost` (ou o nome da sua instância).
   * **Database Name:** O nome do seu banco de dados (ex: `ControleFinanceiro`).
   * **Authentication:** `Integrated` (para Windows Authentication).
   * **Connection Name:** Um nome amigável (ex: `DB_Familia`).

### 3. Executando sua primeira Query
Crie um novo arquivo com a extensão `.sql`. Digite o código e aperte `Ctrl + Shift + E` para executar:

```sql
-- Exemplo de teste
SELECT * FROM MembrosFamilia;
