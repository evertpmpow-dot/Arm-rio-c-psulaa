# Armário do Everton — Cloud Build

Esta versão foi organizada para facilitar a geração do APK em serviços de compilação na nuvem.

## Conteúdo
- Aplicativo Android completo
- 29 peças cadastradas
- Cadastro de novas roupas e fotos
- Gerador de looks
- Favoritos
- Planejador
- Tela Experimentar Look

## Opção mais simples: GitHub Actions

1. Crie uma conta no GitHub.
2. Crie um novo repositório vazio.
3. Envie todos os arquivos desta pasta para o repositório.
4. Abra a aba **Actions**.
5. Escolha **Build Android APK**.
6. Clique em **Run workflow**.
7. Quando terminar, baixe o arquivo **Armario-do-Everton-APK**.

O arquivo gerado será:
`app-debug.apk`

## Serviços de compilação

Também é possível enviar este projeto compactado para um serviço de CI/CD Android que aceite projetos Gradle.

## Estrutura importante

- `app/` — aplicativo
- `app/src/main/assets/index.html` — interface do Armário do Everton
- `.github/workflows/build-apk.yml` — compilação automática na nuvem

## Observação

A versão Debug é indicada para instalação e testes pessoais. Para distribuição oficial é necessário criar e assinar uma versão Release.
