📄 Auto Vitae - Gerador de Currículos Dinâmico
O Auto Vitae é uma aplicação web de página única (Single-Page Application - SPA) que permite criar, editar e exportar currículos profissionais de forma totalmente dinâmica e visual. O grande diferencial é a integração com a Inteligência Artificial, que preenche automaticamente os campos do currículo a partir de textos soltos ou perfis do LinkedIn.

Tudo roda diretamente no seu navegador, sem a necessidade de banco de dados ou servidores back-end.

🚀 Principais Funcionalidades
Preenchimento Mágico com IA: Cole o texto do seu perfil do LinkedIn ou um resumo da sua carreira, e a IA (Google Gemini) extrai e preenche todos os campos do currículo automaticamente.

Edição em Tempo Real: Edite no painel esquerdo e veja o resultado instantaneamente no painel direito.

Múltiplos Layouts: Escolha entre 11 estilos diferentes (Standard, Moderno, Tech/Dev, Criativo, Híbrido, Tradicional, Infográfico, Funcional, Cronológico, Acadêmico e Compacto).

Personalização de Cores e Temas: Altere as cores de destaque e ajuste as escalas (zoom) do conteúdo principal e da barra lateral para garantir que o currículo caiba perfeitamente em uma página.

Gestão de Foto de Perfil: Faça upload da sua foto, ajuste o arredondamento, zoom e a posição (X/Y) diretamente na interface.

Exportação e Importação (JSON): Salve o progresso do seu currículo em um arquivo .json e carregue-o novamente no futuro para atualizações.

Geração de PDF: Exporte o seu currículo pronto para PDF com apenas um clique (usando html2pdf.js ou a impressão nativa do navegador).

Design Responsivo: Interface otimizada para uso tanto em computadores quanto em dispositivos móveis (com visualização em tela cheia).

🛠️ Tecnologias Utilizadas
Este projeto foi construído focado na simplicidade e performance, utilizando um único arquivo HTML:

HTML5 / CSS3 / JavaScript (Vanilla): Lógica e estrutura sem dependência de frameworks complexos como React ou Vue.

Tailwind CSS: Carregado via CDN para estilização rápida, responsiva e moderna.

Lucide Icons: Biblioteca de ícones carregada via CDN.

html2pdf.js: Para renderização e download do currículo em formato PDF.

API do Google Gemini: Utilizada para a funcionalidade de extração e preenchimento inteligente de dados.

📦 Como Usar
Por ser um projeto client-side puro (roda apenas no navegador), a instalação é extremamente simples:

Faça o download: Salve o código fornecido em um arquivo chamado index.html.

Abra no navegador: Dê um clique duplo no arquivo index.html ou arraste-o para dentro do seu navegador favorito (Chrome, Edge, Firefox, Safari).

Comece a editar: Utilize o painel lateral esquerdo para inserir suas informações, adicionar experiências e trocar o layout.

🤖 Como configurar o Preenchimento com IA (Google Gemini)
Para usar o recurso "Preenchimento Mágico", você precisará de uma chave de API gratuita do Google:

Acesse o Google AI Studio.

Faça login com sua conta Google e clique em Create API key.

Copie a chave gerada.

Abra o Auto Vitae, vá na seção de "Preenchimento com IA" e cole a chave no campo indicado pelo ícone de chave (🔑).

Sua chave ficará salva localmente no seu navegador (localStorage) para usos futuros. Nota: A chave nunca é enviada para servidores de terceiros, apenas diretamente para o Google.

🖨️ Dicas de Impressão e PDF
Botão PDF: Utiliza a biblioteca interna para forçar uma página A4 e gerar o arquivo. É excelente para designs mais complexos com cores de fundo.

Impressão Nativa (Ícone de Impressora): Abre a caixa de diálogo nativa do sistema.

Dica: Para que os layouts com fundos coloridos funcionem na impressão nativa, certifique-se de ativar a opção "Imprimir gráficos de fundo" (ou "Background graphics") nas configurações de impressão do seu navegador. Mude as margens para "Nenhuma".

📝 Estrutura de Dados (JSON)
Se desejar exportar seus dados, a aplicação gera um arquivo JSON seguindo este formato base:

JSON
{
  "personal": {
    "name": "Seu Nome",
    "title": "Seu Cargo",
    "email": "email@exemplo.com",
    "phone": "(00) 00000-0000"
  },
  "about": "Resumo profissional...",
  "education": [],
  "practicalTraining": [],
  "skills": [],
  "languages": [],
  "layout": {
    "themeColor": "blue",
    "layoutMode": "moderno"
  }
}
