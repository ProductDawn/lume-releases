# Lume — instaladores para Windows

Este repositório contém apenas os instaladores do Lume, um gestor pessoal de
temas para Windows 11. O código-fonte não está aqui.

O Lume funciona 100% offline: não faz nenhum pedido de rede, não tem contas,
nem sincronização, nem telemetria. Os dados ficam só no PC onde a app é usada.

## Descarregar

As versões estão em **Releases** (barra lateral, à direita). Cada versão tem
três formatos, todos para Windows 11 x64 e sem precisar de administrador:

| Ficheiro | Formato |
|---|---|
| `Lume-Setup-<versão>.exe` | Instalador (recomendado) |
| `Lume-<versão>-win-x64.zip` | Pasta da app, para extrair e abrir |
| `Lume-<versão>-portable.exe` | Portátil, corre sem instalar |
| `SHA256SUMS.txt` | Impressões digitais para confirmar os ficheiros |

As versões 0.x são versões de teste.

## Instalar

- **Instalador:** abrir o ficheiro. Se aparecer "O Windows protegeu o PC",
  escolher *Mais informações* → *Executar mesmo assim* (os instaladores não são
  assinados digitalmente). Instala só para o utilizador atual, em
  `%LOCALAPPDATA%\Programs\Lume`.
- **Zip:** antes de extrair, botão direito → Propriedades → *Desbloquear*.
  Extrair e abrir `Lume.exe`.
- **Portátil:** abrir o ficheiro. Arranca mais devagar, porque se extrai para uma
  pasta temporária a cada arranque.

Os três formatos usam a mesma pasta de dados (`%APPDATA%\Lume`), por isso podem
ser trocados sem perder nada. Para atualizar, basta instalar a versão nova por
cima: os dados mantêm-se.

## Desinstalar

Em Definições → Aplicações. O desinstalador pergunta se deve apagar também os
dados; a resposta por omissão é **Não**.
