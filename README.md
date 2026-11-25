# Experiência MoE

Criei a página **AURELIA — A beleza que respira** com um único prompt para testar o modelo. O objetivo era ver o que ele conseguiria gerar a partir de uma única solicitação.

O resultado é uma landing page responsiva de skincare, com HTML, CSS e JavaScript reunidos em um único arquivo.

## Modelo usado no teste

O **Inkling 2 Mini** é um modelo multimodal de pesos abertos da Thinking Machines Lab, publicado sob a licença Apache 2.0. Ele recebe texto e imagens, gera texto e suporta até 1 milhão de tokens de contexto. A arquitetura *Mixture of Experts* (MoE) tem 26,4 bilhões de parâmetros no total e 3,4 bilhões ativos. Para cada token, o modelo executa as camadas intermediárias três vezes. [Ficha oficial do modelo](https://huggingface.co/thinkingmachines/Inkling-2-Mini)

Para o teste, usei a versão GGUF da Unsloth com quantização dinâmica de 4 bits `UD-Q4_K_XL`. Com **17,63 GB**, ela é a maior variante da faixa de 4 bits listada na ficha da Unsloth. A quantização aplica precisões diferentes aos pesos para reduzir o tamanho do arquivo e limitar a perda de qualidade. [Distribuição GGUF da Unsloth](https://huggingface.co/unsloth/Inkling-2-Mini-GGUF)

## Como visualizar

Baixe o arquivo [`index.html`](index.html) e abra-o no navegador.
