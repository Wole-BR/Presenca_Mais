> **Aviso de Reconstrução de Histórico:**
> *As notas de versão anteriores à 1.10.1 foram redigidas post-mortem para fins de documentação histórica. Este registro serve como linha de base (baseline) para o projeto, consolidando as principais alterações funcionais e estruturais baseadas no conhecimento empírico do desenvolvimento até o momento.*

#### Versões Pré-lançamento (Alpha)
*   **Alpha 1 (Terminal):** Sistema em Python via terminal. Cadastro e armazenamento de alunos feitos exclusivamente através de planilhas.
*   **Alpha 2 (Desktop):** Interface gráfica em PyQt. Utilização de planilhas para entrada de dados (cadastro) e saída (lista de presença e banco de dados).

#### v1.0 - Lançamento Web Inicial
*   **Plataforma:** Migração para interface Web (Site).
*   **Funcionalidades:** Cadastro via planilhas e geração de lista de presença.
*   **Limitação:** Não suporta fotos dos alunos nesta versão.

#### v1.1
*   **Banco de Dados:** Implementação do SQLite para armazenar os dados cadastrados (mantém importação via planilha).
*   **Interface:** Melhorias gerais na UI.
*   **Funcionalidade:** Adicionado suporte para fotos dos alunos.

#### v1.2
*   **Novo Recurso:** Sistema de cadastro manual de alunos (sem necessidade de importação de planilha).

#### v1.3
*   **Personalização:** Implementação do sistema de customização de crachás.

#### v1.4
*   **Atalhos de Teclado:**
    *   `+` : Confirmar presença.
    *   `-` : Cancelar.
    *   `Enter` : Pesquisar aluno.

#### v1.5
*   **Exportação:** Geração de arquivos PDF para impressão dos crachás.

#### v1.6
*   **Backup:**
    *   Implementação de backup automático do SQLite (mantém as 5 versões mais recentes).
    *   Configuração para seleção de pasta de destino do backup.
    *   Recurso para salvar cópia do banco de dados selecionado.

#### v1.7
*   **Design:** Adição de templates de crachás pré-definidos.

#### v1.8
*   **Personalização:** Suporte a crachás em orientação horizontal (seguindo o template).
*   **v1.8.1 (Correção):** Ajuste na centralização do código de barras no crachá.
*   **v1.8.2 (Correção):** Ajustes gerais de interface gráfica.

#### v1.9
*   **Visual:** Substituição de emojis por ícones profissionais.
*   **Identidade:** Adição de suporte para logotipos.

#### v1.10
*   **Hardware:**
    *   Integração com RFID substituindo a exclusividade do código de barras.
    *   Implementação de API Serial (JS) para leitura direta de tags RFID nos campos de input.
*   **Banco de Dados:** Adição de coluna específica para suportar códigos RFID.
*   **v1.10.1 (Correção):** Ajuste no algoritmo de busca na aba "Presença". Corrigido bug onde a validação de limite de caracteres (EAN13) bloqueava leituras de RFID.
