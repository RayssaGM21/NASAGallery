# 🚀 NASA Gallery - Explore o Universo!

Bem-vindo ao **NASA Gallery**! Um projeto incrível onde você pode explorar imagens fascinantes tiradas pela NASA, baseadas no ano do seu aniversário! 🌌🚀

## 🌟 O que é isso?

Este é um site interativo que permite a você viajar pelo universo sem sair de casa! Você pode pesquisar imagens incríveis da NASA por ano, navegar pelas galerias e até visualizar detalhes de cada imagem ao clicar nas miniaturas. Se você já sonhou em ver as maravilhas do cosmos, este é o lugar certo!

### Funcionalidades:
- **Busca por Ano**: Quer ver as fotos do ano do seu aniversário? Basta inserir o ano e explorar as imagens tiradas pela NASA naquele ano!
- **Galeria Interativa**: Explore imagens incríveis da NASA organizadas por página. Navegue por elas e clique em qualquer uma para ver mais detalhes.
- **Navegação Simples**: Com uma navegação fácil e intuitiva, você pode alternar entre as páginas da galeria e visualizar as fotos que mais te interessam.

## 🚀 Como Funciona?

1. **Escolha um Ano**: 
   - Você pode pesquisar por qualquer ano entre 1995 e 2025! Insira o ano e a galeria será atualizada com as imagens daquele ano.
  
2. **Explore as Imagens**:
   - A cada busca, você será apresentado a uma galeria de imagens incríveis da NASA. Explore as miniaturas e clique para ver mais detalhes.
   
3. **Paginação**:
   - As páginas são controladas por um simples sistema de "Anterior" e "Próximo", que permite que você explore as imagens sem se perder.

4. **Clique para Detalhes**:
   - Ao clicar em qualquer imagem, você será levado para uma página de detalhes onde pode ver a foto em maior resolução e ler uma breve descrição sobre ela.

## Como utilizamos a API da NASA no projeto
A API de Imagens da NASA é a fonte principal para trazer imagens espaciais incríveis e outras mídias para o nosso projeto. Aqui está como ela é utilizada:
Api: https://images.nasa.gov/docs/images.nasa.gov_api_docs.pdf

### Busca por Ano

Quando o usuário insere um ano, fazemos uma requisição à API utilizando o endpoint `/search`. Esse endpoint permite buscar imagens do ano especificado, retornando imagens relacionadas àquele ano.

### Parâmetros importantes:
- `year_start` e `year_end`: Filtram as imagens pelo ano.
- `media_type=image`: Filtra para retornar apenas imagens.

### Exemplo de requisição:

```javascript
const response = await fetch(`https://images-api.nasa.gov/search?q=&year_start=${year}&year_end=${year}&media_type=image&page_size=100`);


### Discente: Rayssa Gomides Marconato
### RA: 2001130
