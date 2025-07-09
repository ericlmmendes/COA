Controle Operacional por Agência (COA)
Visão Geral
O Controle Operacional por Agência (COA) é uma aplicação web desenvolvida para otimizar a gestão de colaboradores em operações logísticas. A ferramenta permite registrar informações sobre fornecedores, turnos, quantidades de colaboradores fixos, diaristas, suplentes, faltas, atestados e nomes de colaboradores, gerando relatórios detalhados que podem ser enviados diretamente pelo WhatsApp.
Desenvolvido pela ERICLM, o COA é uma solução prática para empresas que necessitam de controle rigoroso sobre suas equipes operacionais, garantindo precisão e agilidade no registro e compartilhamento de dados.
Funcionalidades

Registro de Dados Operacionais: Formulário intuitivo para inserir informações sobre:
Fornecedor (Enfok, D0, Polly, Blitz)
Data e turno (T1, T2, T3)
Quantidades de colaboradores fixos, diaristas, suplentes, faltas e atestados
Nomes e tipos de colaboradores (Operacional ou Devolução)
Opção de retificação (Sim/Não)


Validação de Formulário: Campos obrigatórios são validados, com bordas vermelhas piscantes para entradas ausentes.
Geração de Relatórios: Relatórios são gerados com base nos dados inseridos, incluindo:
Total de colaboradores presentes (fixos + diaristas - faltas - atestados + suplentes)
Lista de colaboradores separada por tipo (Operacional e Devolução) com numeração (ex.: "1. MANOEL (Operacional)")
Envio direto do relatório via WhatsApp


Interface Responsiva: Design adaptável para dispositivos móveis e desktops, utilizando Tailwind CSS.
Navegação: 
Cabeçalho com logo à esquerda e link "Home" branco à direita.
Rodapé com links para Home, Sobre, Política de Privacidade e Termos de Uso.


Botão de Contato: Botão flutuante do WhatsApp para suporte ou mais informações.

Tecnologias Utilizadas

HTML5: Estrutura das páginas.
React (v18.2.0): Gerenciamento dinâmico do formulário e estado na página principal.
Tailwind CSS: Estilização responsiva e moderna.
Font Awesome (v6.4.2): Ícone do WhatsApp no botão flutuante.
JavaScript (Babel): Transformação de JSX para execução no navegador.
CDN: Dependências hospedadas via cdn.jsdelivr.net e outros provedores.

Estrutura do Projeto
coa/
├── index.html          # Página principal com formulário e geração de relatórios
├── sobre.html          # Página "Sobre" com informações do projeto
├── privacidade.html    # Página de Política de Privacidade
├── termos.html         # Página de Termos de Uso
└── README.md           # Este arquivo

Instalação
O COA é uma aplicação web estática que não requer um servidor backend. Para executá-la localmente:

Clone o Repositório (se hospedado em um sistema de controle de versão):
git clone <URL_DO_REPOSITORIO>
cd coa


Hospede Localmente:

Use um servidor local como o Live Server do VS Code ou qualquer servidor HTTP simples (ex.: python -m http.server 8000).
Abra index.html em um navegador moderno (Chrome, Firefox, etc.).


Dependências:

Todas as dependências (React, Tailwind CSS, Font Awesome) são carregadas via CDN, não sendo necessário instalar pacotes localmente.



Uso

Acesse a Página Principal:

Abra index.html no navegador.
Preencha o formulário com as informações operacionais:
Selecione o fornecedor, data e turno.
Insira as quantidades de fixos, diaristas, suplentes, faltas e atestados.
Adicione nomes de colaboradores e selecione o tipo (Operacional ou Devolução).
Especifique se é uma retificação, se necessário.




Validação:

Campos obrigatórios devem ser preenchidos. Campos vazios serão destacados com bordas vermelhas piscantes.


Geração de Relatório:

Clique no botão "Enviar Relatório para WhatsApp".
Um relatório formatado será gerado, com colaboradores listados por tipo (Operacional e Devolução) e numerados.
O relatório será aberto no WhatsApp para envio.


Navegação:

Use o link "Home" no cabeçalho para voltar à página principal.
Acesse as páginas "Sobre", "Política de Privacidade" e "Termos de Uso" pelo rodapé.
Clique no botão flutuante do WhatsApp para contato com o suporte.



Exemplo de Relatório
*Controle Operacional por Agência - COA*

*Fornecedor:* Enfok
*Data:* 09/07/2025
*Turno:* T1
*Retificação:* Não

*Qt. Fixos:* 10
*Qt. Diaristas:* 5
*Qt. Suplentes:* 2

*Qt. Faltas:* 1
*Qt. Atestados:* 0

*Qt. Fixos + Diaristas (após faltas e atestados):* 14
*Total de Colaboradores Presentes:* 16

*Nomes dos Colaboradores:*
*Operacional:*
1. MANOEL (Operacional)
2. CARLOS (Operacional)

*Devolução:*
1. JOÃO (Devolução)

Contribuição
Contribuições são bem-vindas! Para contribuir:

Faça um fork do repositório.
Crie uma branch para sua feature ou correção:git checkout -b minha-feature


Faça commit das suas alterações:git commit -m "Adiciona minha feature"


Envie para o repositório remoto:git push origin minha-feature


Abra um Pull Request.

Por favor, siga as diretrizes de código, mantendo a consistência com Tailwind CSS e React.
Licença
© 2025 ERICLM. Todos os direitos reservados. Consulte os Termos de Uso para mais detalhes.
Contato
Para suporte ou mais informações, clique no botão flutuante do WhatsApp na aplicação ou envie uma mensagem para o número +55 11 93008-9968.
