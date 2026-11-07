# MENOLI ZB v21 — Pacote organizado

**Comece aqui.** Os arquivos estão separados por destino de uso: plataforma, modelo ou prompt universal. Escolha **uma** dessas opções conforme a sua necessidade.

## Onde encontrar cada coisa?

| Quero usar no… | Abra esta pasta | Como usar |
| --- | --- | --- |
| OpenCode | `01_PLATAFORMAS/01_OpenCode/` | Arquivos prontos para instalar no projeto |
| Codex | `01_PLATAFORMAS/02_Codex/` | Copie `AGENTS.md` para a raiz do projeto |
| Claude Code | `01_PLATAFORMAS/03_Claude_Code/` | Copie `CLAUDE.md` para a raiz do projeto |
| Gemini CLI | `01_PLATAFORMAS/04_Gemini_CLI/` | Copie `GEMINI.md` para a raiz do projeto |
| Cursor | `01_PLATAFORMAS/05_Cursor/` | Copie a pasta `.cursor/` para o projeto |
| GitHub Copilot | `01_PLATAFORMAS/06_GitHub_Copilot/` | Copie a pasta `.github/` para o projeto |
| Outros agentes e editores | `01_PLATAFORMAS/07_Cline/` até `15_AGENTS_MD_Generico/` | Use a pasta específica da sua plataforma |
| ChatGPT | `01_PLATAFORMAS/12_ChatGPT/` | Copie o texto para instruções personalizadas, conforme disponibilidade |
| Gemini no Google AI Studio | `01_PLATAFORMAS/13_Google_AI_Studio/` | Cole no campo de instruções do sistema |
| Claude API | `01_PLATAFORMAS/14_Anthropic_API/` | Utilize o texto como instrução de sistema na sua integração |
| Um modelo específico | `02_MODELOS/` | Abra a subpasta do fornecedor e selecione o arquivo `.md` |
| Um prompt genérico | `03_PROMPTS_UNIVERSAIS/` | Escolha completo, rápido ou aprofundado |

### Pastas principais

```text
MENOLI_ZB_v21_ORGANIZADO/
├── COMECE_AQUI.md             ← este guia
├── instalar.py                ← instalador opcional para plataformas
├── 01_PLATAFORMAS/            ← 15 destinos: OpenCode, Codex, Claude Code…
├── 02_MODELOS/                ← 48 perfis em 9 fornecedores
└── 03_PROMPTS_UNIVERSAIS/     ← 3 versões para copiar e colar
```

## Instalar com um comando (Linux, macOS ou Windows com Python)

No terminal, dentro desta pasta, execute:

```bash
python3 instalar.py --list
python3 instalar.py --platform opencode --dest ~/meu-projeto
```

Troque `opencode` por `codex`, `claude-code`, `gemini-cli`, `cursor`, `copilot` etc. Troque `~/meu-projeto` pela pasta do seu projeto. No Windows, use `python` em vez de `python3` caso seja esse o nome do executável.

- **Padrão seguro:** não substitui arquivos existentes. Em caso de conflito, informa os caminhos e cancela antes de copiar.
- **Substituição opcional:** `--force` substitui e cria backup com sufixo `.bak` quando não existe backup anterior.
- **Atenção:** um `opencode.json` já existente pode conter outras configurações; prefira mesclar manualmente em vez de substituí-lo.
- Os arquivos ocultos `.opencode`, `.github` e `.cursor` são necessários para o funcionamento de algumas plataformas. Ative a visualização de arquivos ocultos no gerenciador se precisar vê-los.

## Qual prompt universal escolher?

- **01_COMPLETO.md:** uso cotidiano e tarefas de programação em geral.
- **02_RAPIDO.md:** modelos leves ou respostas com menor sobrecarga de instruções.
- **03_APROFUNDADO.md:** projetos grandes, análise e implementação em várias etapas.

**Nota:** os 48 nomes na pasta `02_MODELOS` são rótulos herdados de perfis, não confirmação de que cada nome seja um ID oficial de API. Instruções `.md` não alteram privilégios ou restrições da plataforma.
