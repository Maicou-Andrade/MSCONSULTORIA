# Guia de Migração de Site Estático Criado com Manus

Este guia tem como objetivo fornecer informações e passos para migrar um site estático criado com a plataforma Manus para outros serviços de hospedagem.



## O que é um Site Estático?

Um site estático é composto por arquivos HTML, CSS e JavaScript que são entregues ao navegador do usuário exatamente como estão armazenados no servidor. Diferente de sites dinâmicos (que usam bancos de dados e linguagens de programação no servidor, como PHP ou Python), sites estáticos não precisam de processamento no lado do servidor para gerar as páginas. Isso os torna mais rápidos, seguros e fáceis de hospedar, pois exigem menos recursos e podem ser servidos diretamente de uma rede de entrega de conteúdo (CDN).

Sites criados com a Manus, como o seu, são geralmente sites estáticos, o que facilita muito a sua portabilidade para outras plataformas de hospedagem.



## Como Obter os Arquivos do Seu Site Manus

Para migrar seu site, o primeiro passo é obter todos os arquivos estáticos (HTML, CSS, JavaScript, imagens, etc.) que compõem o seu site. Atualmente, a Manus não oferece uma funcionalidade direta de download de todos os arquivos do site. No entanto, você pode:

1.  **Copiar o código-fonte manualmente:** Para sites menores, você pode inspecionar o código-fonte de cada página no seu navegador (clicando com o botão direito e selecionando 'Inspecionar' ou 'Ver código-fonte da página') e salvar o HTML, CSS e JavaScript em arquivos locais. As imagens e outros ativos precisarão ser baixados separadamente.

2.  **Usar ferramentas de download de sites:** Existem ferramentas de terceiros (como `wget` para linha de comando ou softwares de download de sites) que podem 'espelhar' um site, baixando todos os seus arquivos. No entanto, é importante ter cuidado ao usar essas ferramentas e verificar se todos os arquivos foram baixados corretamente e se os caminhos relativos estão funcionando.

3.  **Solicitar à equipe Manus (se disponível):** Em alguns casos, a equipe de suporte da Manus pode ser capaz de fornecer um pacote com todos os arquivos do seu site. Esta seria a opção mais garantida para obter uma cópia completa e correta do seu site.

Após obter todos os arquivos, organize-os em uma pasta local no seu computador, mantendo a estrutura de diretórios original.



## Opções de Hospedagem para Sites Estáticos

Sites estáticos são muito flexíveis em termos de hospedagem, pois não exigem um servidor com processamento de backend. Existem diversas opções, desde serviços gratuitos até plataformas pagas com recursos avançados. Algumas das opções mais populares e recomendadas incluem:

### Serviços Gratuitos e de Baixo Custo:

*   **GitHub Pages:** Ideal para desenvolvedores, permite hospedar sites estáticos diretamente de um repositório GitHub. É gratuito e fácil de usar para projetos pessoais ou de código aberto.
*   **Netlify:** Oferece uma plataforma de hospedagem e implantação contínua para sites estáticos, com um plano gratuito generoso. Possui integração com Git e CDN global para alta performance.
*   **Vercel:** Similar ao Netlify, focado em desenvolvimento frontend e implantação de sites estáticos e aplicações serverless. Também oferece um plano gratuito e CDN.
*   **Cloudflare Pages:** Outra opção para implantação de sites estáticos diretamente de repositórios Git, com CDN global e recursos de segurança da Cloudflare.
*   **Firebase Hosting (Google):** Parte da plataforma Firebase do Google, oferece hospedagem rápida e segura para conteúdo web estático e dinâmico, com um nível gratuito.

### Serviços de Nuvem (Pagos, mas com Nível Gratuito ou Baixo Custo):

*   **AWS S3 (Amazon Web Services):** Um serviço de armazenamento de objetos que pode ser configurado para hospedar sites estáticos. É muito escalável e econômico para grandes volumes de tráfego, mas exige um pouco mais de configuração.
*   **Google Cloud Storage:** Similar ao AWS S3, permite hospedar sites estáticos em buckets de armazenamento. Também é escalável e oferece um nível gratuito.
*   **Azure Static Web Apps (Microsoft Azure):** Uma solução completa para hospedar sites estáticos com integração Git, APIs serverless e CDN.

### Provedores de Hospedagem Tradicionais:

*   Muitos provedores de hospedagem compartilhada (Hostinger, KingHost, etc.) também permitem hospedar sites estáticos. Basta fazer o upload dos arquivos para a pasta `public_html` ou equivalente. Esta pode ser uma boa opção se você já tiver uma conta de hospedagem com um desses provedores.

## Passos para Migrar Seu Site:

1.  **Escolha um Provedor:** Com base nas suas necessidades (custo, facilidade de uso, recursos adicionais), escolha o serviço de hospedagem que melhor se adapta a você.
2.  **Crie uma Conta:** Registre-se no provedor escolhido.
3.  **Faça o Upload dos Arquivos:** A maioria dos provedores oferece uma interface web (FTP ou painel de controle) para fazer o upload dos seus arquivos. Se você estiver usando um serviço como GitHub Pages, Netlify ou Vercel, o processo geralmente envolve conectar seu repositório Git e a plataforma fará a implantação automaticamente.
4.  **Configure o Domínio (Opcional):** Se você tiver um domínio personalizado, siga as instruções do seu provedor de hospedagem para apontá-lo para o seu novo site.
5.  **Teste o Site:** Após a implantação, verifique se todas as páginas, links e funcionalidades estão funcionando corretamente no novo ambiente.

Espero que este guia seja útil para você migrar seu site! Se tiver mais alguma dúvida, pode perguntar.

