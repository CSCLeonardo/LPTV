# LPTV

O **LPTV** é um aplicativo Android para organizar e reproduzir filmes, séries e canais ao vivo em um só lugar. Com uma interface escura e detalhes em vermelho, reúne navegação por categorias, busca, favoritos, histórico e downloads para assistir offline.

## Como funciona

O aplicativo acessa o catálogo disponibilizado pelo servidor configurado ou por uma lista M3U informada pelo usuário no modo convidado. A partir dessa fonte, organiza os conteúdos e permite escolher o que assistir.

A disponibilidade de filmes, séries, canais, capas e informações depende da fonte utilizada. O LPTV funciona como um reprodutor e organizador: o código do aplicativo não inclui os arquivos de vídeo do catálogo.

## Formas de acesso

- **Conta:** acesso com login e senha ao catálogo disponibilizado pelo servidor.
- **Convidado:** entrada por URL de lista M3U, com histórico e favoritos separados da conta do servidor.

## Navegação e descoberta

### Tela inicial

A Home reúne filmes e séries em alta, a seção **Continuar assistindo** e opções para explorar o catálogo por serviços de streaming.

### Filmes e séries

O catálogo pode ser explorado por categorias ou pela busca por título. A navegação por páginas carrega os resultados conforme o uso, sem exigir que todo o catálogo seja carregado de uma vez.

A categoria **Lançamentos** reúne os grupos de diferentes anos, apresentando primeiro os anos mais recentes. Nas séries, os episódios são organizados por temporada.

### Canais ao vivo e jogos do dia

A área de canais permite acessar as transmissões ao vivo disponíveis na fonte configurada. A tela **Jogos do dia** oferece acesso aos canais relacionados aos eventos disponibilizados pela integração.

## Reprodução

A página de cada título apresenta as capas e as informações disponíveis no catálogo. Quando não há uma imagem de fundo disponível, a capa principal pode ser usada desfocada para compor a tela.

O usuário pode iniciar a reprodução ou retomar um conteúdo pela seção **Continuar assistindo**. O aplicativo mantém o progresso e o registro do que foi assistido, além de controlar a abertura do player para evitar sessões duplicadas.

### Assistir na TV

O LPTV possui integração com **Chromecast e DLNA** para reprodução em dispositivos compatíveis na mesma rede. O funcionamento depende do receptor, da conexão e do formato disponibilizado pela fonte.

## Favoritos e histórico

- **Favoritos:** reúne filmes e séries marcados pelo usuário para facilitar o acesso depois.
- **Histórico:** permite consultar os conteúdos assistidos, com abas de filmes e séries.
- **Limpeza do histórico:** considera a aba, o texto da busca e o período selecionado, preservando os conteúdos fora desses filtros.

## Downloads e modo offline

Filmes e episódios podem ser baixados para reprodução local. A tela **Downloads** separa os conteúdos nas abas Filmes e Séries e apresenta duas situações:

| Seção | Conteúdo |
| --- | --- |
| **Pendentes** | Itens aguardando na fila ou em transferência, com acompanhamento do progresso e opção de cancelar. |
| **Baixados** | Conteúdos concluídos e disponíveis para reprodução local. |

A fila transfere **um arquivo por vez**. Ao concluir, o conteúdo passa para os baixados; os episódios ficam organizados na série e na temporada correspondentes.

Os downloads preservam o arquivo fornecido pela origem, sem conversão de resolução ou compressão adicional. A qualidade e o tamanho dependem do link disponibilizado.

Para assistir sem internet, o conteúdo precisa estar baixado no dispositivo. Capas e informações armazenadas em cache não substituem o arquivo de vídeo.

## Armazenamento e carregamento

O aplicativo utiliza armazenamento local e cache para reaproveitar dados e capas, reduzindo consultas repetidas. As buscas e a navegação do catálogo consultam os resultados conforme a necessidade.

O primeiro carregamento de imagens e a reprodução online dependem da velocidade da conexão e da resposta da fonte de conteúdo.

## Tecnologias

| Camada | Tecnologia |
| --- | --- |
| Interface | React Native e React |
| Lógica da interface | TypeScript |
| Integrações Android | Java |
| Reprodução de vídeo | AndroidX Media3 / ExoPlayer |
| Chromecast | Google Cast Framework |
| Carregamento de imagens nativas | Glide |
| Compilação Android | Gradle |

## Plataforma

Desenvolvido para **Android 8.0 ou superior**, com interface principal em orientação vertical e layout adaptável ao tamanho da tela.
