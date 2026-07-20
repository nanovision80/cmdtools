# 🚀 Expansão da Curadoria de Ferramentas de Linha de Comando (CLI)

Novas ferramentas selecionadas para complementar a curadoria original, incluindo líderes de mercado em nichos específicos e alternativas emergentes com foco em performance e IA.

---

## 🎬 Manipulação de Mídia (Vídeo, Áudio e Imagem)

- **vips (libvips)** (Manipulação de Imagem): Biblioteca e CLI de processamento de imagens com uso de memória e velocidade drasticamente superiores ao ImageMagick em imagens grandes.
  - *Ponto Forte:* Processa imagens gigantes (mapas, scans, satélite) sem estourar RAM, graças ao processamento em streaming/pipeline.
  - *Público-alvo:* Desenvolvedores backend que processam imagens em massa ou em produção.

- **realesrgan-ncnn-vulkan** (Manipulação de Imagem / IA): Ferramenta de upscaling de imagem baseada em redes neurais (Real-ESRGAN), rodando via CLI com aceleração Vulkan.
  - *Ponto Forte:* Amplia resolução de imagens/frames de vídeo com qualidade muito superior a algoritmos tradicionais de interpolação.
  - *Público-alvo:* Editores de vídeo, restauradores de imagem e entusiastas de IA generativa.

- **oxipng** (Otimização de Imagem): Otimizador de PNG escrito em Rust, focado em compressão sem perdas ultrarrápida.
  - *Ponto Forte:* Multithreaded e significativamente mais rápido que o clássico `optipng`, mantendo a mesma taxa de compressão.
  - *Público-alvo:* Desenvolvedores web e pipelines de CI/CD que otimizam assets automaticamente.

- **chafa** (Visualização de Imagem): Renderiza imagens e GIFs diretamente no terminal usando caracteres Unicode/ANSI/Sixel.
  - *Ponto Forte:* Permite visualizar previews de imagens sem sair da linha de comando, com suporte a terminais modernos (Kitty, iTerm2).
  - *Público-alvo:* Desenvolvedores que trabalham 100% via SSH/terminal remoto.

- **whisper.cpp** (Transcrição de Áudio / IA): Implementação em C/C++ ultraleve do modelo Whisper da OpenAI para transcrição de áudio offline.
  - *Ponto Forte:* Roda localmente sem GPU dedicada, sem enviar dados sensíveis para APIs externas.
  - *Público-alvo:* Jornalistas, criadores de conteúdo e devs que precisam de transcrição privada e offline.

---

## 🌐 Redes, Downloads e APIs

- **xh** (Cliente HTTP): Alternativa ao HTTPie escrita em Rust, com sintaxe compatível mas performance de inicialização muito superior.
  - *Ponto Forte:* Combina a usabilidade do HTTPie com a velocidade nativa do Rust — ideal para scripts que fazem muitas chamadas.
  - *Público-alvo:* Desenvolvedores de API que buscam um HTTPie mais rápido.

- **ngrok** (Túneis e Exposição de Rede): Cria túneis seguros que expõem um servidor local para a internet instantaneamente.
  - *Ponto Forte:* Simplicidade de um único comando para testar webhooks e demos sem configurar DNS ou firewall.
  - *Público-alvo:* Desenvolvedores full-stack testando integrações externas (Stripe, Twilio, etc.).

- **grpcurl** (Teste de API): O equivalente do `curl` para serviços gRPC, permitindo inspecionar e invocar endpoints gRPC.
  - *Ponto Forte:* Suporta reflection de serviço, eliminando a necessidade de arquivos `.proto` locais.
  - *Público-alvo:* Engenheiros de backend/microsserviços que trabalham com gRPC.

- **rustscan** (Segurança/Varredura): Scanner de portas ultrarrápido escrito em Rust que alimenta os resultados diretamente no Nmap.
  - *Ponto Forte:* Varre todas as 65535 portas em segundos, muito mais rápido que o Nmap sozinho.
  - *Público-alvo:* Pentesters e profissionais de segurança ofensiva.

- **doggo** (DNS): Cliente de linha de comando para consultas DNS, com saída colorida e legível, substituindo o `dig`.
  - *Ponto Forte:* Interface humanizada e suporte nativo a DoH (DNS over HTTPS), algo que o `dig` não oferece nativamente.
  - *Público-alvo:* SREs e administradores de rede.

---

## 📂 Manipulação e Processamento de Dados

- **miller (mlr)** (Processamento de Dados): "Canivete suíço" para CSV, TSV e JSON, combinando funções de `awk`, `sed`, `cut` e `join` em um único formato agnóstico.
  - *Ponto Forte:* Manipula dados tabulares heterogêneos com uma sintaxe unificada, sem precisar alternar entre ferramentas.
  - *Público-alvo:* Analistas de dados e engenheiros que lidam com ETL leve via terminal.

- **visidata (vd)** (Exploração de Dados): Ferramenta de planilha interativa em terminal para navegar, filtrar e analisar grandes datasets tabulares.
  - *Ponto Forte:* Abre CSVs de milhões de linhas instantaneamente, algo que travaria o Excel/Google Sheets.
  - *Público-alvo:* Cientistas de dados e analistas que exploram dados brutos rapidamente.

- **dasel** (Seletor de Dados): Ferramenta universal (query e edição) para JSON, YAML, TOML e XML com uma sintaxe única, semelhante ao `jq`.
  - *Ponto Forte:* Converte entre formatos e edita in-place sem precisar de ferramentas diferentes para cada tipo de arquivo.
  - *Público-alvo:* Engenheiros DevOps lidando com arquivos de configuração heterogêneos.

- **sd** (Busca e Substituição): Alternativa intuitiva ao `sed` para find-and-replace, com sintaxe muito mais simples e regex por padrão.
  - *Ponto Forte:* Elimina a necessidade de escapar caracteres especiais constantemente, reduzindo erros comuns do `sed`.
  - *Público-alvo:* Desenvolvedores que fazem refatorações rápidas via terminal.

- **jless** (Visualizador JSON): Pager interativo para JSON, navegável com teclas estilo VI, otimizado para arquivos JSON enormes.
  - *Ponto Forte:* Colapsa/expande estruturas profundas com fluidez, superando o `fx` em datasets muito grandes.
  - *Público-alvo:* Desenvolvedores backend depurando respostas de API complexas.

---

## 🖥️ Monitoramento de Sistema e Recursos

- **bottom (btm)** (Monitoramento): Monitor de sistema multiplataforma em Rust, com gráficos de CPU/memória/rede em tempo real.
  - *Ponto Forte:* Extremamente customizável via arquivo de configuração, com temas e layouts flexíveis.
  - *Público-alvo:* Desenvolvedores que querem um `htop`/`btop` altamente personalizável.

- **nvtop** (Monitoramento de GPU): Equivalente do `htop` para GPUs, exibindo uso, temperatura e processos em placas NVIDIA/AMD/Intel.
  - *Ponto Forte:* Essencial para monitorar cargas de treinamento de IA/ML em tempo real, algo que ferramentas genéricas não cobrem.
  - *Público-alvo:* Engenheiros de Machine Learning e quem treina modelos localmente.

- **dust (du-dust)** (Uso de Disco): Alternativa moderna ao `du`, exibindo uma árvore visual intuitiva de uso de espaço em disco.
  - *Ponto Forte:* Saída em árvore instantânea e legível, sem precisar combinar `du` com `sort` manualmente.
  - *Público-alvo:* Qualquer usuário de terminal que precisa liberar espaço rapidamente.

- **bandwhich** (Monitoramento de Rede): Exibe em tempo real qual processo está consumindo a largura de banda da rede.
  - *Ponto Forte:* Associa tráfego de rede diretamente a processos e conexões, algo que `iostat`/`htop` não fazem.
  - *Público-alvo:* Administradores de sistema diagnosticando consumo anômalo de rede.

- **zenith** (Monitoramento): Monitor de sistema em Rust com gráficos históricos "zoomable" de CPU, memória, rede e disco.
  - *Ponto Forte:* Permite voltar no tempo e analisar picos de uso passados, não apenas o instante atual.
  - *Público-alvo:* SREs investigando degradação de performance ao longo do tempo.

---

## ⚡ Produtividade, Navegação e Utilitários

- **zellij** (Multiplexador de Terminal): Alternativa moderna ao `tmux`, com layouts predefinidos e curva de aprendizado mais suave.
  - *Ponto Forte:* Interface descobrível com dicas de atalhos na tela, reduzindo a necessidade de memorizar comandos.
  - *Público-alvo:* Desenvolvedores que acham o `tmux` pouco intuitivo.

- **yazi** (Gerenciador de Arquivos): Gerenciador de arquivos de terminal escrito em Rust, com preview de imagens/vídeos assíncrono.
  - *Ponto Forte:* Extremamente rápido mesmo em diretórios com milhares de arquivos, com preview nativo de mídia.
  - *Público-alvo:* Usuários avançados que querem substituir o `ranger` por algo mais performático.

- **atuin** (Histórico de Shell): Substitui o histórico padrão do shell por um banco de dados SQLite pesquisável e sincronizável entre máquinas.
  - *Ponto Forte:* Busca contextual (por diretório, exit code, horário) e sincronização criptografada entre dispositivos.
  - *Público-alvo:* Desenvolvedores que trabalham em múltiplas máquinas/servidores.

- **starship** (Prompt de Shell): Prompt customizável, rápido e agnóstico de shell (Bash, Zsh, Fish, PowerShell).
  - *Ponto Forte:* Detecta automaticamente contexto do projeto (linguagem, branch Git, versão) sem configuração complexa.
  - *Público-alvo:* Todo desenvolvedor que quer um terminal mais informativo e bonito.

- **navi** (Cheatsheets Interativos): Cheatsheet interativo que permite buscar e executar comandos complexos preenchendo variáveis via prompt.
  - *Ponto Forte:* Diferente do `tldr` (que só exibe), o `navi` executa o comando escolhido diretamente no terminal.
  - *Público-alvo:* Devs que esquecem flags de comandos complexos (Docker, ffmpeg, etc.).

---

## 🛠️ Desenvolvimento, Versionamento e Automação

- **mise** (Gerenciador de Versões): Gerenciador polivalente de runtimes (Node, Python, Ruby, Go etc.), substituindo `nvm`, `pyenv` e `asdf` em uma única ferramenta.
  - *Ponto Forte:* Muito mais rápido que `asdf` (escrito em Rust) e gerencia variáveis de ambiente por projeto como o `direnv`.
  - *Público-alvo:* Desenvolvedores full-stack que alternam entre múltiplas linguagens e projetos.

- **difftastic** (Diff Estrutural): Ferramenta de diff que entende a sintaxe do código (AST), em vez de comparar linha por linha.
  - *Ponto Forte:* Ignora mudanças cosméticas (formatação, reindentação) e destaca apenas alterações semânticas reais.
  - *Público-alvo:* Desenvolvedores revisando pull requests com refatorações grandes.

- **git-delta** (Visualização de Diff): Substitui o output padrão do `git diff` por uma versão com syntax highlighting e visualização lado a lado.
  - *Ponto Forte:* Integra-se diretamente ao Git/GitHub CLI, tornando diffs muito mais legíveis no terminal.
  - *Público-alvo:* Times que revisam código extensivamente via terminal.

- **tokei** (Estatísticas de Código): Conta linhas de código, comentários e espaços em branco por linguagem, instantaneamente.
  - *Ponto Forte:* Extremamente rápido (Rust) mesmo em repositórios enormes, suportando mais de 150 linguagens.
  - *Público-alvo:* Tech leads avaliando tamanho/complexidade de um repositório.

- **watchexec** (Automação): Executa comandos automaticamente sempre que arquivos são modificados, sem precisar configurar watchers manuais.
  - *Ponto Forte:* Agnóstico de linguagem e stack — funciona para rodar testes, builds ou linters em qualquer projeto.
  - *Público-alvo:* Desenvolvedores em fluxos de desenvolvimento com live-reload.

---

## 🤖 Inteligência Artificial no Terminal (Nova Categoria)

- **ollama** (Execução de LLMs Locais): CLI para baixar e rodar modelos de linguagem open-source (Llama, Mistral, Gemma) localmente.
  - *Ponto Forte:* Abstrai toda a complexidade de quantização e inferência em um único comando (`ollama run`).
  - *Público-alvo:* Desenvolvedores que querem IA local, privada e offline.

- **llm** (Interface Universal de LLMs): CLI criada por Simon Willison para interagir com diversos modelos (OpenAI, Anthropic, locais) em um só lugar.
  - *Ponto Forte:* Suporta plugins, embeddings e logging de conversas em SQLite, funcionando como um hub unificado de IA.
  - *Público-alvo:* Desenvolvedores que testam/comparam múltiplos provedores de LLM.

- **aider** (Pareamento de Código com IA): Ferramenta de terminal que edita arquivos de um repositório Git diretamente a partir de instruções em linguagem natural.
  - *Ponto Forte:* Aplica e commita mudanças automaticamente, mantendo um histórico Git limpo do que a IA alterou.
  - *Público-alvo:* Desenvolvedores que querem um "par de programação" via IA sem sair do terminal.

- **fabric** (Automação de Prompts): Framework open-source que organiza "patterns" (prompts reutilizáveis) para tarefas como resumir, extrair insights ou revisar texto via CLI.
  - *Ponto Forte:* Cria um pipeline reutilizável de prompts versionados, em vez de reescrever prompts do zero toda vez.
  - *Público-alvo:* Power users que automatizam fluxos de trabalho intelectuais com IA.

- **shell-gpt (sgpt)** (Assistente de Shell): Integra modelos de linguagem diretamente ao shell, gerando e explicando comandos a partir de linguagem natural.
  - *Ponto Forte:* Converte descrições em português/inglês diretamente em comandos shell prontos para execução.
  - *Público-alvo:* Usuários que esquecem sintaxes complexas de `find`, `awk` ou `ffmpeg`.
