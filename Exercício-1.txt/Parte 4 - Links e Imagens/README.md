# Documentação da Parte 4 - Links e Imagens

Este diretório armazena a atividade prática relacionada ao uso de hiperlinks e exibição de imagens em HTML.

## Como corrigir uma imagem quebrada no HTML?

Caso uma imagem não carregue no navegador (fique "quebrada"), as seguintes etapas devem ser seguidas para identificar e corrigir o problema:

1. **Verificar o Caminho do Arquivo (`src`):** Certificar-se de que a rota passada no atributo `src` corresponde à localização real do arquivo. Caminhos relativos devem considerar onde o `index.html` está localizado em relação à imagem (ex: `img/nome.jpg`).
2. **Checar Extensões e Letras Maiúsculas/Minúsculas:** Sistemas baseados em Linux (como os servidores de hospedagem e o GitHub) são *case-sensitive*. Portanto, `imagem.jpg` é diferente de `imagem.JPG` ou `imagem.jpeg`.
3. **Validar a Existência do Arquivo:** Confirmar se o arquivo de imagem foi de fato movido para a pasta correta (`img/`) e se ele não foi deletado acidentalmente.
4. **Verificar o Nome do Arquivo:** Evitar o uso de espaços em branco, acentos ou caracteres especiais no nome dos arquivos de imagem (prefira nomes como `foto-perfil.jpg` em vez de `foto perfil.jpg`).
