📄 Auto Vitae - Gerador de Currículos Dinâmico
O Auto Vitae é uma aplicação web de página única (Single-Page Application - SPA) que permite criar, editar e exportar currículos profissionais de forma totalmente dinâmica e visual. O grande diferencial é a integração com a Inteligência Artificial, que preenche automaticamente os campos do currículo a partir de textos soltos ou perfis do LinkedIn.

Tudo roda diretamente no seu navegador, sem a necessidade de banco de dados ou servidores back-end.

🚀 Principais Funcionalidades
Preenchimento Mágico: Cole suas informações e o Auto Vitae detecta palavras chaves para extrair e preencher os campos do currículo automaticamente.

**Edição em Tempo Real**: Edite no painel esquerdo e veja o resultado instantaneamente no painel direito (**Personalização de Cores e Temas, Gestão de Foto de Perfil, Exportação e Importação (JSON), Geração de PDF.**).
Design Responsivo: Interface otimizada para uso tanto em computadores quanto em dispositivos móveis (com visualização em tela cheia).

📦 Como Usar
Por ser um projeto client-side puro (roda apenas no navegador), a instalação é extremamente simples:
1. Faça o download
2. Salve o código fornecido em um arquivo chamado index.html
3. Abra no navegador: Dê um clique duplo no arquivo index.html ou arraste-o para dentro do seu navegador favorito (Chrome, Edge, Firefox, Safari).
ou acesse o site na página do github: **https://brad38.github.io/Auto-Vitae/**

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
