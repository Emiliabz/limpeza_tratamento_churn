
📊 Análise de Churn: Telecomunicações

📝 Descrição do Projeto
Este projeto consiste em um estudo de caso detalhado sobre a evasão de clientes (Churn) em uma empresa de telecomunicações. O foco principal é a aplicação de técnicas rigorosas de limpeza e tratamento de dados para preparar a base para futuras análises exploratórias e modelos de Machine Learning.

Desenvolvido durante o curso "Pandas: limpeza e tratamento de dados" da Alura, o projeto aborda desafios reais de dados sujos, como estruturas JSON aninhadas, outliers e valores ausentes.

🛠️ Tecnologias e Bibliotecas
- Pandas: Manipulação e estruturação dos dados.

- NumPy: Operações matemáticas e tratamento de arrays.

- Seaborn & Matplotlib: Visualização de dados e identificação visual de outliers.

- JSON: Processamento de arquivos de dados semiestruturados.

📁 O Conjunto de Dados
- O arquivo dataset-telecon.json contém informações críticas, incluindo:

- Demográficos: Dados sobre o perfil do cliente.

- Serviços: Tipos de contratos e serviços assinados.

- Financeiro: Métodos de pagamento e cobranças mensais/totais.

- Target: Status de Churn (se o cliente deixou ou não a empresa).

⚙️ Etapas de Pré-processamento
O pipeline de tratamento seguiu as seguintes fases:

- Normalização: Transformação da estrutura JSON aninhada em um DataFrame plano via pd.json_normalize().

- Sanitização Financeira: Correção da coluna de cobranças totais e ajuste do tempo de serviço para contratos específicos.

- Gestão de Nulos: Remoção estratégica de linhas com dados cruciais ausentes e imputação calculada para o tempo de serviço.

- Deduplicação: Identificação e remoção de registros duplicados.

- Tratamento de Outliers: Aplicação do método IQR (Intervalo Interquartil) para detectar e corrigir valores atípicos no tempo de serviço.

- Feature Engineering:

- Remoção de IDs irrelevantes.

- Codificação binária (0 e 1) para variáveis sim/não.

0 Aplicação de One-Hot Encoding (variáveis dummy) para colunas multicategóricas.

🚀 Como Executar
Clone o repositório:

Bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
Instale as dependências:

Bash
pip install pandas numpy seaborn matplotlib
Dataset:
Certifique-se de que o arquivo dataset-telecon.json esteja na raiz do projeto.

Execute o Notebook:
Abra o seu ambiente favorito (Jupyter, VS Code ou Colab) e execute as células sequencialmente.
-------------------------------------------------------------------------------------------------
⭐ Este projeto faz parte do meu processo de transição de carreira para a área de Dados.
