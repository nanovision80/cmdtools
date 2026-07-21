# 🚀 Curadoria de Ferramentas de Linha de Comando (CLI)

Uma coleção selecionada com mais de 80 ferramentas de linha de comando indispensáveis para desenvolvedores, administradores de sistema e entusiastas de tecnologia. Divididas por categorias para facilitar a navegação.

---

## 🎬 Manipulação de Mídia (Vídeo, Áudio e Imagem)

- **[ffmpeg](https://ffmpeg.org/)** — O canivete suíço para converter, gravar e transmitir áudio e vídeo. Suporta praticamente todos os formatos existentes e é a base de incontáveis pipelines de processamento de mídia.

- **[exiftool](https://exiftool.org/)** — Leitura, escrita e edição de metadados em uma enorme variedade de arquivos (imagens, vídeos, áudios, PDFs etc.). Essencial para forense digital e organização de bibliotecas de mídia.

- **[imagemagick](https://imagemagick.org/)** — Criação, edição, composição e conversão de imagens bitmap. A ferramenta de referência para manipulação de imagens via linha de comando há décadas.

- **[yt-dlp](https://github.com/yt-dlp/yt-dlp)** — Utilitário robusto para baixar vídeos e áudios do YouTube e de centenas de outros sites. Fork ativo e bem mantido do youtube-dl com suporte a novos formatos.

- **[graphicsmagick](http://www.graphicsmagick.org/)** — Alternativa derivada do ImageMagick, focada em maior velocidade e eficiência, especialmente em operações em lote.

- **[sox](http://sox.sourceforge.net/)** — O "FFmpeg dos arquivos de áudio", ideal para ler, escrever e processar efeitos sonoros, conversões e análise de áudio.

- **[gifsicle](https://www.lcdf.org/gifsicle/)** — Criação, edição e otimização pesada de animações em formato GIF. Permite reduzir drasticamente o tamanho de GIFs sem perda perceptível de qualidade.

- **[svgo](https://github.com/svg/svgo)** — Otimizador de arquivos SVG baseado em Node.js. Remove metadados desnecessários e simplifica paths para SVGs mais leves em produção web.

- **[vips (libvips)](https://www.libvips.org/)** — Biblioteca e CLI de processamento de imagens com uso de memória e velocidade drasticamente superiores ao ImageMagick em imagens grandes. Processa imagens gigantes (mapas, scans, satélite) sem estourar RAM, graças ao processamento em streaming/pipeline. Ideal para desenvolvedores backend que processam imagens em massa ou em produção.

- **[realesrgan-ncnn-vulkan](https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan)** — Ferramenta de upscaling de imagem baseada em redes neurais (Real-ESRGAN), rodando via CLI com aceleração Vulkan. Amplia resolução de imagens/frames de vídeo com qualidade muito superior a algoritmos tradicionais de interpolação. Perfeita para editores de vídeo, restauradores de imagem e entusiastas de IA generativa.

- **[oxipng](https://github.com/shssoichiro/oxipng)** — Otimizador de PNG escrito em Rust, focado em compressão sem perdas ultrarrápida. Multithreaded e significativamente mais rápido que o clássico `optipng`, mantendo a mesma taxa de compressão. Essencial para desenvolvedores web e pipelines de CI/CD que otimizam assets automaticamente.

- **[chafa](https://github.com/hpjansson/chafa)** — Renderiza imagens e GIFs diretamente no terminal usando caracteres Unicode/ANSI/Sixel. Permite visualizar previews de imagens sem sair da linha de comando, com suporte a terminais modernos (Kitty, iTerm2). Ideal para desenvolvedores que trabalham 100% via SSH/terminal remoto.

- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Implementação em C/C++ ultraleve do modelo Whisper da OpenAI para transcrição de áudio offline. Roda localmente sem GPU dedicada, sem enviar dados sensíveis para APIs externas. Perfeita para jornalistas, criadores de conteúdo e devs que precisam de transcrição privada e offline.

---

## 🌐 Redes, Downloads e APIs

- **[curl](https://curl.se/)** — Transferência de dados usando sintaxe de URL (HTTP, FTP, IMAP, etc.), essencial para testar APIs e automatizar downloads. Presente em praticamente todos os sistemas Unix.

- **[wget](https://www.gnu.org/software/wget/)** — Download não interativo de arquivos da web, excelente para downloads recursivos, espelhamento de sites e scripts de automação.

- **[httpie](https://httpie.io/)** — Um cliente HTTP de linha de comando moderno, amigável e com destaque de sintaxe por padrão. Torna o teste de APIs uma experiência visualmente agradável.

- **[nmap](https://nmap.org/)** — Ferramenta de exploração de rede, varredura de portas e auditoria de segurança. O padrão ouro para reconhecimento de rede e descoberta de serviços.

- **[mtr](https://www.bitwizard.nl/mtr/)** — Combina a funcionalidade dos comandos `traceroute` e `ping` em uma única ferramenta de diagnóstico de rede em tempo real.

- **[aria2](https://aria2.github.io/)** — Utilitário leve de download multiprotocolo que suporta links HTTP/HTTPS, FTP, BitTorrent e Metalink. Permite downloads paralelos e retomada de downloads interrompidos.

- **[speedtest-cli](https://github.com/sivel/speedtest-cli)** — Interface de linha de comando para testar a largura de banda da sua internet usando o Speedtest.net. Útil para monitoramento e automação de testes de velocidade.

- **[socat](http://www.dest-unreach.org/socat/)** — Conector multipropósito que estabelece dois fluxos de dados bidirecionais entre diferentes tipos de canais (sockets, arquivos, pipes, dispositivos seriais etc.).

- **[xh](https://github.com/ducaale/xh)** — Alternativa ao HTTPie escrita em Rust, com sintaxe compatível mas performance de inicialização muito superior. Combina a usabilidade do HTTPie com a velocidade nativa do Rust — ideal para scripts que fazem muitas chamadas.

- **[ngrok](https://ngrok.com/)** — Cria túneis seguros que expõem um servidor local para a internet instantaneamente. Simplicidade de um único comando para testar webhooks e demos sem configurar DNS ou firewall. Essencial para desenvolvedores full-stack testando integrações externas (Stripe, Twilio, etc.).

- **[grpcurl](https://github.com/fullstorydev/grpcurl)** — O equivalente do `curl` para serviços gRPC, permitindo inspecionar e invocar endpoints gRPC. Suporta reflection de serviço, eliminando a necessidade de arquivos `.proto` locais. Indispensável para engenheiros de backend/microsserviços que trabalham com gRPC.

- **[rustscan](https://github.com/RustScan/RustScan)** — Scanner de portas ultrarrápido escrito em Rust que alimenta os resultados diretamente no Nmap. Varre todas as 65535 portas em segundos, muito mais rápido que o Nmap sozinho. Ferramenta essencial para pentesters e profissionais de segurança ofensiva.

- **[doggo](https://github.com/mr-karan/doggo)** — Cliente de linha de comando para consultas DNS, com saída colorida e legível, substituindo o `dig`. Interface humanizada e suporte nativo a DoH (DNS over HTTPS), algo que o `dig` não oferece nativamente. Ideal para SREs e administradores de rede.

---

## 📂 Manipulação e Processamento de Dados

- **[jq](https://github.com/jqlang/jq)** — Processador de dados JSON flexível, ideal para filtrar, mapear e transformar objetos complexos diretamente no terminal.

- **[ripgrep (rg)](https://github.com/BurntSushi/ripgrep)** — Uma alternativa ultrarrápida ao `grep` que respeita seus arquivos `.gitignore` por padrão e é otimizada para busca em código-fonte.

- **[fzf](https://github.com/junegunn/fzf)** — Localizador interativo (fuzzy finder) de uso geral para arquivos, histórico de comandos e processos. Integra-se perfeitamente a qualquer workflow de terminal.

- **[sed](https://www.gnu.org/software/sed/)** — Editor de fluxo de texto usado para realizar transformações básicas em um fluxo de entrada. O clássico indispensável para manipulação de texto.

- **[awk](https://www.gnu.org/software/gawk/)** — Linguagem de programação versátil projetada para processamento de padrões e dados textuais. Poderosa para extração e transformação de dados tabulares.

- **[bat](https://github.com/sharkdp/bat)** — Um clone do comando `cat` com realce de sintaxe integrado e integração com o Git. Mostra diffs, números de linha e paging automático.

- **[fx](https://github.com/antonmedv/fx)** — Visualizador JSON interativo de terminal que permite expandir e recolher nós facilmente. Ótimo para explorar estruturas JSON complexas.

- **[xsv](https://github.com/BurntSushi/xsv)** — CLI rápida para indexação, fatiamento, análise e junção de arquivos CSV. Escrita em Rust para máxima performance.

- **[yq](https://github.com/mikefarah/yq)** — Um wrapper portátil de linha de comando para o `jq`, adaptado para arquivos YAML, XML e TOML. Permite query e transformação de dados em múltiplos formatos.

- **[miller (mlr)](https://github.com/johnkerl/miller)** — "Canivete suíço" para CSV, TSV e JSON, combinando funções de `awk`, `sed`, `cut` e `join` em um único formato agnóstico. Manipula dados tabulares heterogêneos com uma sintaxe unificada, sem precisar alternar entre ferramentas. Perfeito para analistas de dados e engenheiros que lidam com ETL leve via terminal.

- **[visidata (vd)](https://www.visidata.org/)** — Ferramenta de planilha interativa em terminal para navegar, filtrar e analisar grandes datasets tabulares. Abre CSVs de milhões de linhas instantaneamente, algo que travaria o Excel/Google Sheets. Essencial para cientistas de dados e analistas que exploram dados brutos rapidamente.

- **[dasel](https://github.com/TomWright/dasel)** — Ferramenta universal (query e edição) para JSON, YAML, TOML e XML com uma sintaxe única, semelhante ao `jq`. Converte entre formatos e edita in-place sem precisar de ferramentas diferentes para cada tipo de arquivo. Ideal para engenheiros DevOps lidando com arquivos de configuração heterogêneos.

- **[sd](https://github.com/chmln/sd)** — Alternativa intuitiva ao `sed` para find-and-replace, com sintaxe muito mais simples e regex por padrão. Elimina a necessidade de escapar caracteres especiais constantemente, reduzindo erros comuns do `sed`. Perfeito para desenvolvedores que fazem refatorações rápidas via terminal.

- **[jless](https://jless.io/)** — Pager interativo para JSON, navegável com teclas estilo VI, otimizado para arquivos JSON enormes. Colapsa/expande estruturas profundas com fluidez, superando o `fx` em datasets muito grandes. Essencial para desenvolvedores backend depurando respostas de API complexas.

---

## 🖥️ Monitoramento de Sistema e Recursos

- **[htop](https://htop.dev/)** — Visualizador de processos interativo e colorido, uma evolução direta do clássico `top` com suporte a mouse e árvore de processos.

- **[btop](https://github.com/aristocratos/btop)** — Monitor de recursos impressionante e altamente visual que exibe CPU, memória, discos e rede com gráficos detalhados e tema customizável.

- **[duf](https://github.com/muesli/duf)** — Utilitário moderno de uso de disco que exibe informações de forma clara e colorida, substituindo o `df` com uma interface muito mais legível.

- **[ncdu](https://dev.yorhel.nl/ncdu)** — Analisador de uso de disco baseado em texto (ncurses), perfeito para encontrar o que está ocupando espaço em servidores remotos.

- **[glances](https://github.com/nicolargo/glances)** — Monitor de sistema multiplataforma baseado em Python que condensa dezenas de métricas em uma tela, com modo cliente/servidor e API REST.

- **[fastfetch](https://github.com/fastfetch-cli/fastfetch)** — Ferramenta de informação do sistema altamente customizável e rápida (sucessor espiritual do `neofetch`). Exibe informações do sistema com estilo.

- **[procs](https://github.com/dalance/procs)** — Um substituto moderno para o comando `ps`, escrito em Rust, com cores, busca aprimorada e exibição de informações adicionais como portas TCP.

- **[iostat](https://docs.oracle.com/cd/E23824_01/html/821-1461/iostat-1m.html)** — Monitor de carga de dispositivos de armazenamento do sistema e uso de CPU. Parte do pacote sysstat, essencial para diagnóstico de performance de I/O.

- **[bottom (btm)](https://github.com/ClementTsang/bottom)** — Monitor de sistema multiplataforma em Rust, com gráficos de CPU/memória/rede em tempo real. Extremamente customizável via arquivo de configuração, com temas e layouts flexíveis. Ideal para desenvolvedores que querem um `htop`/`btop` altamente personalizável.

- **[nvtop](https://github.com/Syllo/nvtop)** — Equivalente do `htop` para GPUs, exibindo uso, temperatura e processos em placas NVIDIA/AMD/Intel. Essencial para monitorar cargas de treinamento de IA/ML em tempo real, algo que ferramentas genéricas não cobrem. Indispensável para engenheiros de Machine Learning e quem treina modelos localmente.

- **[dust (du-dust)](https://github.com/bootandy/dust)** — Alternativa moderna ao `du`, exibindo uma árvore visual intuitiva de uso de espaço em disco. Saída em árvore instantânea e legível, sem precisar combinar `du` com `sort` manualmente. Perfeito para qualquer usuário de terminal que precisa liberar espaço rapidamente.

- **[bandwhich](https://github.com/imsnif/bandwhich)** — Exibe em tempo real qual processo está consumindo a largura de banda da rede. Associa tráfego de rede diretamente a processos e conexões, algo que `iostat`/`htop` não fazem. Essencial para administradores de sistema diagnosticando consumo anômalo de rede.

- **[zenith](https://github.com/bvaisvil/zenith)** — Monitor de sistema em Rust com gráficos históricos "zoomable" de CPU, memória, rede e disco. Permite voltar no tempo e analisar picos de uso passados, não apenas o instante atual. Ideal para SREs investigando degradação de performance ao longo do tempo.

---

## ⚡ Produtividade, Navegação e Utilitários

- **[tldr](https://github.com/tldr-pages/tldr)** — Páginas de manual simplificadas e focadas na comunidade, mostrando apenas exemplos práticos de uso. O complemento perfeito para manpages tradicionais.

- **[zoxide](https://github.com/ajeetdsouza/zoxide)** — Um substituto inteligente para o comando `cd` que aprende seus hábitos para navegar mais rápido entre diretórios frequentemente acessados.

- **[eza](https://github.com/eza-community/eza)** — Um substituto moderno, customizável e cheio de recursos para o tradicional comando `ls`, com ícones, cores Git e mais.

- **[tmux](https://github.com/tmux/tmux)** — Multiplexador de terminal que permite gerenciar várias sessões e janelas em uma única tela. Essencial para trabalho remoto e organização de múltiplos contextos.

- **[rclone](https://rclone.org/)** — Sincroniza arquivos e diretórios de/para dezenas de serviços de armazenamento em nuvem (Drive, S3, Dropbox, etc.). O canivete suíço para backups e migração na nuvem.

- **[pandoc](https://pandoc.org/)** — O conversor de documentos universal, transformando Markdown, PDF, DOCX, HTML e mais. Indispensável para geração de documentação e publicações acadêmicas.

- **[trash-cli](https://github.com/andreafrancia/trash-cli)** — Envia arquivos para a lixeira do sistema em vez de deletá-los permanentemente com o `rm`. Segurança contra exclusões acidentais.

- **[micro](https://github.com/zyedidia/micro)** — Editor de texto moderno baseado em terminal, intuitivo e com suporte nativo a atalhos padrão (Ctrl+C, Ctrl+V). Ideal para quem não domina Vim/Emacs.

- **[ranger](https://github.com/ranger/ranger)** — Gerenciador de arquivos de terminal com mapeamento de teclas VI e visualização prévia de arquivos. Navegação eficiente pelo sistema de arquivos.

- **[zellij](https://github.com/zellij-org/zellij)** — Alternativa moderna ao `tmux`, com layouts predefinidos e curva de aprendizado mais suave. Interface descobrível com dicas de atalhos na tela, reduzindo a necessidade de memorizar comandos. Perfeito para desenvolvedores que acham o `tmux` pouco intuitivo.

- **[yazi](https://github.com/sxyazi/yazi)** — Gerenciador de arquivos de terminal escrito em Rust, com preview de imagens/vídeos assíncrono. Extremamente rápido mesmo em diretórios com milhares de arquivos, com preview nativo de mídia. Ideal para usuários avançados que querem substituir o `ranger` por algo mais performático.

- **[atuin](https://github.com/atuinsh/atuin)** — Substitui o histórico padrão do shell por um banco de dados SQLite pesquisável e sincronizável entre máquinas. Busca contextual (por diretório, exit code, horário) e sincronização criptografada entre dispositivos. Perfeito para desenvolvedores que trabalham em múltiplas máquinas/servidores.

- **[starship](https://github.com/starship/starship)** — Prompt customizável, rápido e agnóstico de shell (Bash, Zsh, Fish, PowerShell). Detecta automaticamente contexto do projeto (linguagem, branch Git, versão) sem configuração complexa. Todo desenvolvedor que quer um terminal mais informativo e bonito deve experimentar.

- **[navi](https://github.com/denisidoro/navi)** — Cheatsheet interativo que permite buscar e executar comandos complexos preenchendo variáveis via prompt. Diferente do `tldr` (que só exibe), o `navi` executa o comando escolhido diretamente no terminal. Ideal para devs que esquecem flags de comandos complexos (Docker, ffmpeg, etc.).

---

## 🛠️ Desenvolvimento, Versionamento e Automação

- **[git](https://git-scm.com/)** — O sistema de controle de versão distribuído padrão de mercado. A base de todo workflow de desenvolvimento moderno.

- **[gh](https://github.com/cli/cli)** — A interface de linha de comando oficial do GitHub para gerenciar Issues, Pull Requests e Repositórios diretamente do terminal.

- **[make](https://www.gnu.org/software/make/)** — Utilitário de automação de compilação que determina automaticamente quais partes de um programa precisam ser recriadas. Ainda relevante após décadas.

- **[direnv](https://github.com/direnv/direnv)** — Extensão para o seu shell que carrega e descarrega variáveis de ambiente dependendo do diretório atual. Essencial para gerenciar múltiplos projetos com dependências diferentes.

- **[hyperfine](https://github.com/sharkdp/hyperfine)** — Ferramenta de benchmarking de linha de comando estatística para medir o tempo de execução de comandos com precisão e comparações justas.

- **[shellcheck](https://github.com/koalaman/shellcheck)** — Ferramenta de análise estática (linter) que encontra bugs e avisa sobre más práticas em scripts Bash/Sh. Indispensável para scripts em produção.

- **[lazygit](https://github.com/jesseduffield/lazygit)** — Interface visual simples de terminal para comandos Git, ideal para quem quer agilizar o fluxo de trabalho sem decorar comandos complexos.

- **[act](https://github.com/nektos/act)** — Execute suas ações do GitHub Actions localmente dentro do terminal usando containers Docker. Teste seus workflows CI/CD antes de pushar.

- **[mise](https://github.com/jdx/mise)** — Gerenciador polivalente de runtimes (Node, Python, Ruby, Go etc.), substituindo `nvm`, `pyenv` e `asdf` em uma única ferramenta. Muito mais rápido que `asdf` (escrito em Rust) e gerencia variáveis de ambiente por projeto como o `direnv`. Perfeito para desenvolvedores full-stack que alternam entre múltiplas linguagens e projetos.

- **[difftastic](https://github.com/Wilfred/difftastic)** — Ferramenta de diff que entende a sintaxe do código (AST), em vez de comparar linha por linha. Ignora mudanças cosméticas (formatação, reindentação) e destaca apenas alterações semânticas reais. Ideal para desenvolvedores revisando pull requests com refatorações grandes.

- **[git-delta](https://github.com/dandavison/delta)** — Substitui o output padrão do `git diff` por uma versão com syntax highlighting e visualização lado a lado. Integra-se diretamente ao Git/GitHub CLI, tornando diffs muito mais legíveis no terminal. Essencial para times que revisam código extensivamente via terminal.

- **[tokei](https://github.com/XAMPPRocky/tokei)** — Conta linhas de código, comentários e espaços em branco por linguagem, instantaneamente. Extremamente rápido (Rust) mesmo em repositórios enormes, suportando mais de 150 linguagens. Perfeito para tech leads avaliando tamanho/complexidade de um repositório.

- **[watchexec](https://github.com/watchexec/watchexec)** — Executa comandos automaticamente sempre que arquivos são modificados, sem precisar configurar watchers manuais. Agnóstico de linguagem e stack — funciona para rodar testes, builds ou linters em qualquer projeto. Ideal para desenvolvedores em fluxos de desenvolvimento com live-reload.

---

## 🤖 Inteligência Artificial no Terminal

- **[ollama](https://github.com/ollama/ollama)** — CLI para baixar e rodar modelos de linguagem open-source (Llama, Mistral, Gemma) localmente. Abstrai toda a complexidade de quantização e inferência em um único comando (`ollama run`). Perfeito para desenvolvedores que querem IA local, privada e offline.

- **[llm](https://github.com/simonw/llm)** — CLI criada por Simon Willison para interagir com diversos modelos (OpenAI, Anthropic, locais) em um só lugar. Suporta plugins, embeddings e logging de conversas em SQLite, funcionando como um hub unificado de IA. Ideal para desenvolvedores que testam/comparam múltiplos provedores de LLM.

- **[aider](https://github.com/paul-gauthier/aider)** — Ferramenta de terminal que edita arquivos de um repositório Git diretamente a partir de instruções em linguagem natural. Aplica e commita mudanças automaticamente, mantendo um histórico Git limpo do que a IA alterou. Perfeito para desenvolvedores que querem um "par de programação" via IA sem sair do terminal.

- **[fabric](https://github.com/danielmiessler/fabric)** — Framework open-source que organiza "patterns" (prompts reutilizáveis) para tarefas como resumir, extrair insights ou revisar texto via CLI. Cria um pipeline reutilizável de prompts versionados, em vez de reescrever prompts do zero toda vez. Ideal para power users que automatizam fluxos de trabalho intelectuais com IA.

- **[shell-gpt (sgpt)](https://github.com/TheR1D/shell_gpt)** — Integra modelos de linguagem diretamente ao shell, gerando e explicando comandos a partir de linguagem natural. Converte descrições em português/inglês diretamente em comandos shell prontos para execução. Perfeito para usuários que esquecem sintaxes complexas de `find`, `awk` ou `ffmpeg`.

---

> **Dica:** A maioria dessas ferramentas está disponível nos gerenciadores de pacotes oficiais das principais distribuições Linux (apt, dnf, pacman, brew) e pode ser instalada com um único comando. Para as ferramentas em Rust, considere usar `cargo install` ou `cargo binstall` quando o pacote não estiver disponível no repositório da sua distro.
