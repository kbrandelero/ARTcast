# ARTCast — atualizações

Arquivos que o plugin **ARTCast** (Revit 2026, Artesul) lê ao abrir o Revit para se atualizar sozinho:

- `atualizacao/versao.txt` — 1ª linha = versão publicada; `sha256=` da DLL; `notas=` do que mudou.
- `atualizacao/ARTCast.dll` — a DLL dessa versão.

Se a versão publicada for maior que a instalada, o plugin baixa a DLL, confere o SHA-256 e pergunta se reinicia o Revit.
Publicação: `scripts/dev/publicar_versao.ps1` no projeto do ARTCast.
