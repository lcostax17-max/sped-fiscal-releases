# Gerador de SPED — releases públicas

Este repositório guarda só os **arquivos de distribuição** do Gerador de SPED:

- **`latest.json`** — manifesto que o programa lê para saber se há versão nova
  (versão, o que muda, link do instalador e checksum).
- **Releases** — cada release traz o instalador `GeradorSPED_Setup.exe`.

O **código-fonte é privado**; aqui ficam apenas o instalador e a lista de versões.

## Baixar / instalar

Pegue o instalador mais recente em **[Releases](../../releases/latest)** e rode o
`GeradorSPED_Setup.exe`. Depois de instalado, o programa avisa sozinho quando
sai uma versão nova (mostrando o que muda, e só atualiza se você aceitar).

## Para o mantenedor (publicar uma versão)

1. Gere o instalador no projeto e calcule o `sha256`.
2. Crie a release com o instalador como anexo:
   `gh release create vX.Y instalador/GeradorSPED_Setup.exe --repo lcostax17-max/sped-fiscal-releases`
3. Atualize o `latest.json` (versão, notas, sha256) e dê push na `main`.
