# 🎙️ Wispr Local — ditado por voz pro Mac

Fale em vez de digitar, **em qualquer aplicativo**: aperte o atalho, fale, aperte de novo — o texto (já corrigido pela IA, se você quiser) entra sozinho no campo onde seu cursor está. Funciona no WhatsApp Web, Mail, Notion, navegador, onde for.

- ✅ Transcrição **100% local** no seu Mac (funciona até sem internet)
- ✅ Ajuste opcional por IA (corrigir, resumir, virar e-mail…) com **prompt seu**
- ✅ Fica na barra de cima (ícone de ondinha), leve (~0% de CPU parado)
- ✅ Suas chaves de API e textos **nunca saem do seu Mac**

**Requisito:** macOS 14 (Sonoma) ou mais novo.

---

## 📥 Instalação (2 minutos)

1. **Baixe** o [`Wispr-Local-1.0.zip`](Wispr-Local-1.0.zip?raw=true) (clique e depois em "Download").
2. Dê **dois cliques no zip** — vai aparecer o `Wispr Local.app`.
3. **Arraste o `Wispr Local.app` pra pasta Aplicativos.**
4. ⚠️ **Primeira abertura** (só na primeira vez): o macOS vai dizer que não conhece o desenvolvedor. Faça assim:
   - Clique no app com o **botão direito → Abrir → Abrir**.
   - Se ainda assim não abrir: **Ajustes do Sistema → Privacidade e Segurança**, role até o fim e clique em **"Abrir Mesmo Assim"**.
5. O app aparece como um **ícone de ondinha 🎙️ na barra de cima** da tela (não fica no Dock — é proposital, ele vive em segundo plano).

## 🔓 Permissões (uma vez só)

Clique no ícone da ondinha → **⚙️ Configurar** → botão **"Ativar 'Digitar no campo' (Acessibilidade)"** → ligue o **Wispr Local** na lista que abrir.
Na primeira gravação, o macOS ainda vai pedir **Microfone** e **Reconhecimento de Fala** — é só permitir.

> Sem a Acessibilidade, o atalho global e a inserção automática do texto não funcionam.

## 🚀 Como usar

1. Clique num campo de texto de qualquer app (um e-mail, uma mensagem…).
2. Aperte o atalho — o padrão é **fn + Tab** (dá pra trocar: ⚙️ → "Gravar atalho" → aperte a combinação que quiser).
3. **Fale.** Aparece um microfone vermelho piscando embaixo, no centro da tela.
4. Aperte o atalho **de novo** → o texto entra sozinho no campo. 🎉
5. Falou besteira? **Esc** cancela (e aparece um botão "Desfazer" se mudar de ideia).

## 🤖 Ajuste por IA (opcional, mas é o pulo do gato)

No ⚙️ Configurar:
- Cole sua **chave da OpenAI** (`sk-...`, em [platform.openai.com/api-keys](https://platform.openai.com/api-keys)) e/ou da **Anthropic** (`sk-ant-...`, em [console.anthropic.com](https://console.anthropic.com/settings/keys)).
- No campo **Prompt**, diga o que a IA deve fazer com sua fala. Ex.: *"Mantenha o que eu falei, tirando redundância e corrigindo pontuação, em português."* Tem atalhos prontos: **Resumir**, **Corrigir**, **E-mail**.
- Em **"Ajuste por IA ao inserir pelo atalho"**, escolha qual IA usa. O padrão é **"Nenhum"** (insere o texto cru, sem custo) — troque pra GPT/Claude/Automático se quiser o ajuste.

Sem chave nenhuma o app funciona normal — só insere a transcrição sem ajuste.

## ⚙️ Outras opções

| Opção | Onde | Pra quê |
|---|---|---|
| Abrir no login | ⚙️ Configurar | O app sobe sozinho quando você liga o Mac |
| Motor de transcrição | ⚙️ Configurar | **SpeechAnalyzer** (padrão — motor novo da Apple; precisa de **macOS 26**; em versões anteriores o app usa o Local sozinho) · **Local** (clássico, rápido/offline) · **Nuvem/IA** (OpenAI, mais preciso, precisa de chave) |
| Histórico | Janela principal | Últimas transcrições, com "Usar" e "Copiar" |
| Sair | Janela principal | Encerra o app de vez |

## ❓ Problemas comuns

- **"O texto não entra no campo"** → falta a permissão de Acessibilidade (veja acima). Ligou e nada? Feche e abra o app.
- **"O atalho não faz nada"** → mesma coisa: Acessibilidade. Depois de ligar, clique no ícone da ondinha uma vez (ele rearma o atalho).
- **"Não transcreve em português"** → o pacote de voz pt-BR baixa sozinho na primeira vez; aguarde uns segundos com internet ligada.

---

*Dúvidas? Abra uma [Issue](../../../issues).*
