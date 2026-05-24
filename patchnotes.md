# Patch Notes — CloakBrowser

**Data:** 2026-05-24 (atividade local)  
**Commit local HEAD:** `8028dde` — `feat: route HTTP proxy credentials through --proxy-server`  
**Branch:** `main`  
**Remote:** `https://github.com/LucasOl1337/CloakBrowser.git` (fork) · upstream `CloakHQ/CloakBrowser`

---

## Resumo

Nenhum commit local do usuário nesta janela de 24h. A atividade local foi limitada a **`profiles/`** (sessões de browser — excluídas do git por segurança). O HEAD atual aponta para o commit upstream de proxy credentials de 2026-05-21.

---

## Último commit no repositório (upstream)

### Added / Changed

- Roteamento de credenciais HTTP proxy via `--proxy-server`
- `cloakbrowser/browser.py` — suporte expandido a proxy com autenticação
- `js/src/proxy.ts`, `js/src/puppeteer.ts` — integração JS/TS
- Testes ampliados: `js/tests/proxy.test.ts`, `tests/test_proxy.py`, `tests/test_persistent_context.py`

## Atividade local (2026-05-24)

- Diretório `profiles/` modificado — perfis persistentes de browser (Google, etc.)
- **Não commitado** — contém cookies/sessões sensíveis

## Notes

- Para publicar alterações locais de perfis, usar backup externo — nunca versionar `profiles/`
- Considere adicionar `profiles/` ao `.gitignore` se ainda não estiver coberto
