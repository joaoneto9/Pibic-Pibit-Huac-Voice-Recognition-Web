# Pibic-Pibit-Huac-Voice-Recognition-Web

- [Instalando das Dependencias](#Instalacao-das-Dependencias)
- [Como Rodar a aplicacao e informacoes do IP e da Porta](#Como-Rodar-a-aplicacao-e-informacoes-do-IP-e-da-Porta)
- [Documentacao das consulta ao Backend](#Documentacao-das-consulta-ao-Backend)
---

Aplicacao web desenvolvida para transcrissoes de audio, aonde buscamos entender o funcionamento de requisicoes
web com audios e como a gerar um fluxograma concreto dessa informacao ate a obtencao do texto transcrito.

### Instalacao das Dependencias

1. Este projeto exige versões específicas do ambiente de execução para garantir a compatibilidade das dependências.
Versões Mínimas

      Node.js: v20.0.0 (LTS) ou superior
  
      npm: v10.0.0 ou superior

2. Instalação ou Atualização do Node.js
Caso não possua o NVM instalado:

**O nvm (Node Version Manager) é essencial para gerenciar versões sem conflitos de permissão.**

**Windows: Baixe e execute o nvm-setup.exe em [nvm-setup.exe](https://github.com/coreybutler/nvm-windows/releases)**

**macOS/Linux: Instale via curl:**
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```
3. Com o NVM instalado:

Execute os comandos para instalar e utilizar a versão estável mais recente:
```
nvm install --lts
nvm use --lts
```
4. Atualização do npm

Após garantir que o Node.js está na versão LTS, atualize o gerenciador de pacotes globalmente:

```
npm install -g npm@latest
```

5. Instalando as dependencias da aplicacao:

Va ate o diretorio da aplicacao e rode o comando:
```
cd ./web-voice-recognition
npm install 
```

### Como Rodar a aplicacao e informacoes do IP e da Porta

1. Rodando a aplicacao:

Ja estando no diretorio - `./web-voice-recognition`- da aplicacao, rode:
```
npm run dev
```

2. Informacoes de IP e Porta

Apos a inicializacao da aplicacao, a aplicacao estara rodando no `localhost` na porta `5173`:
[http://localhost:5173/](http://localhost:5173/)

### Documentacao das consulta ao Backend

Para realizar a requisição ao backend, é necessário compreender que o envio de dados em formato Blob 
(objetos JavaScript que representam arquivos binários, como o `.webm` neste contexto) exige o uso do objeto FormData.

<img width="627" height="473" alt="image" src="https://github.com/user-attachments/assets/b6e9315f-1005-4b14-8206-a65a99f54516" />

- Uso do FormData: Como o áudio é um arquivo binário (Blob), utiliza-se o FormData para "empacotar" esse arquivo de um jeito
que o servidor consiga entender.

- Automação do Navegador: Ao passar esse pacote para a função fetch, o navegador configura automaticamente os detalhes técnicos
(como o tipo de conteúdo e os limites do arquivo), garantindo que o áudio chegue íntegro ao backend sem muitas configuracoes.

### Colaboradores:

- [guinoronhaf](https://github.com/guinoronhaf)
- [joaoneto9](https://github.com/joaoneto9)
- [rebecasouzag](https://github.com/joaoneto9)

