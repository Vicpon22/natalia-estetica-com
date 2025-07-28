# Configuração do Domínio Personalizado no GitHub Pages

## Instruções para Configurar o Subdomínio `cslqnopp.natalia.esteticaprofissional`

Para hospedar seu site no GitHub Pages com o subdomínio `cslqnopp.natalia.esteticaprofissional`, siga os passos abaixo:

### 1. Configuração do Repositório GitHub

1.  **Crie um novo repositório no GitHub** (ou use um existente) para o seu site. O nome do repositório pode ser qualquer um, por exemplo, `natalia-estetica-portfolio`.
2.  **Faça upload de todos os arquivos do projeto** (incluindo o `index.html`, `css/`, `js/`, `images/`, `assets/` e o arquivo `CNAME` que está neste ZIP) para a raiz do seu repositório no GitHub.

### 2. Configuração do GitHub Pages

1.  No seu repositório GitHub, vá para **Settings** (Configurações).
2.  No menu lateral, clique em **Pages**.
3.  Em 

Source`, selecione a branch `main` (ou a branch onde seu código está) e a pasta `/ (root)`.
4.  Em `Custom domain`, digite `cslqnopp.natalia.esteticaprofissional` e clique em `Save`.

### 3. Configuração DNS no seu Provedor de Domínio

Esta é a parte mais importante. Você precisará acessar o painel de controle do seu provedor de domínio (onde você comprou `natalia.esteticaprofissional`).

1.  **Adicione um registro CNAME** para o subdomínio `cslqnopp`:
    -   **Tipo**: `CNAME`
    -   **Nome/Host**: `cslqnopp`
    -   **Valor/Destino**: `<SEU_USUARIO_GITHUB>.github.io` (substitua `<SEU_USUARIO_GITHUB>` pelo seu nome de usuário do GitHub)
    -   **TTL**: 300 (ou o padrão)

    **Exemplo**: Se seu usuário GitHub for `meuusuario`, o valor/destino será `meuusuario.github.io`.

2.  **Aguarde a propagação do DNS**: Pode levar de alguns minutos a 48 horas para que as alterações de DNS se propaguem globalmente.

### 4. Verificação e HTTPS

1.  Após a propagação, tente acessar `https://cslqnopp.natalia.esteticaprofissional` no seu navegador.
2.  No GitHub Pages, na seção `Custom domain`, marque a opção `Enforce HTTPS` para garantir que seu site seja acessado via HTTPS (pode levar um tempo para ficar disponível após a configuração do domínio).

## Arquivos do Projeto

-   O código do site já está preparado para o novo subdomínio.
-   O arquivo `CNAME` na raiz do projeto já contém `cslqnopp.natalia.esteticaprofissional`.
-   As meta tags no `index.html` foram atualizadas para refletir o novo subdomínio.

## Estrutura dos Arquivos

```
natalia-estetica-com/
├── index.html          # Página principal
├── css/
│   └── style.css       # Estilos customizados
├── js/
│   └── script.js       # JavaScript interativo
├── images/             # Imagens do site
├── assets/             # Recursos adicionais
├── CNAME               # Arquivo para configuração do domínio no GitHub Pages
└── CONFIGURACAO_DOMINIO.md # Este arquivo de instruções
```

## Suporte

Se precisar de ajuda com a configuração DNS ou com o GitHub Pages, consulte a documentação oficial do GitHub Pages ou entre em contato com o suporte do seu provedor de domínio.

