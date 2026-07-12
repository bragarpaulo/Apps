# 👁️ Mac Spy — monitor leve para o Mac

Veja CPU, memória e processos diretamente na barra superior do macOS. O Mac Spy funciona localmente, abre um painel compacto ao clicar e não envia dados para a internet.

- ✅ CPU e memória na barra superior
- ✅ Escolha quais métricas e ícones aparecem
- ✅ Lista pesquisável de processos com ícones dos aplicativos
- ✅ Gráficos, categorias de carga e ordenação por CPU ou memória
- ✅ Encerramento normal ou forçado, sempre manual e com confirmação
- ✅ Coletor nativo otimizado, sem abrir `ps`, `vm_stat` ou processos auxiliares

**Requisitos:** macOS 13 ou mais novo e Mac com Apple Silicon (M1, M2, M3, M4 ou posterior).

---

## 📥 Instalação

1. **Baixe** o [`Mac-Spy-1.4.1.zip`](Mac-Spy-1.4.1.zip?raw=true).
2. Dê dois cliques no ZIP para obter `Mac Spy.app`.
3. Arraste `Mac Spy.app` para a pasta **Aplicativos**.
4. Na primeira abertura, clique no app com o **botão direito → Abrir → Abrir**.
5. Se o macOS ainda bloquear: abra **Ajustes do Sistema → Privacidade e Segurança** e clique em **Abrir Mesmo Assim**.

O Mac Spy não aparece no Dock. Ele fica na barra superior, ao lado dos indicadores do sistema.

## 🚀 Como usar

### Abrir o painel

- **Clique esquerdo** no indicador da barra para abrir ou fechar o painel.
- **Clique direito** para abrir o menu rápido com configurações e a opção **Encerrar Mac Spy**.

### Barra superior

No menu `•••` do painel ou no clique direito da barra, configure:

| Configuração | Efeito |
|---|---|
| Exibir CPU | Mostra o percentual de CPU na barra |
| Exibir memória | Mostra o percentual de memória na barra |
| Ícone da CPU | Mostra ou oculta o símbolo de processador |
| Ícone da memória | Mostra ou oculta o símbolo de memória |
| Ordem das métricas | Define CPU ou memória primeiro |
| Atualização automática | Liga ou pausa a coleta periódica |

Pelo menos uma métrica permanece visível para o app não desaparecer da barra.

### Processos

- Use a busca para localizar um aplicativo pelo nome ou PID.
- Clique em **CPU** ou **MEM** para alterar a ordenação.
- Os pontos coloridos classificam a carga: crítico, alto, moderado, leve ou ocioso.
- Clique com o botão direito em um processo para mostrar seu executável no Finder ou solicitar encerramento.
- O botão **Forçar encerramento** deve ser usado somente quando o encerramento normal não funcionar.

## ⚙️ Padrões da versão 1.4.1

- CPU visível
- Memória oculta
- Ícones de CPU e memória ocultos
- CPU primeiro
- Atualização automática ativa
- Painel fechado: atualização leve de CPU/memória a cada 8 segundos
- Painel aberto: processos atualizados a cada 3 segundos

As alterações feitas nos menus são salvas no Mac e recuperadas na próxima abertura.

## 🪶 Desempenho

Com o painel fechado, o Mac Spy consulta somente CPU e memória pelas APIs nativas do macOS. A lista de processos, os gráficos e os ícones são carregados apenas quando o painel é aberto e são liberados ao fechar.

O cache de ícones é limitado a 2 MB. Não existem processos auxiliares executados periodicamente.

## 🔒 Privacidade e segurança

- Todos os dados permanecem no Mac.
- O app não possui telemetria nem conexão de rede.
- Nenhum processo é encerrado, suspenso ou desacelerado automaticamente.
- Um processo só recebe comando de encerramento depois de uma ação explícita e confirmação.
- Processos protegidos pelo macOS podem apresentar informações limitadas ou recusar encerramento.

## ❓ Problemas comuns

- **O indicador não apareceu:** abra novamente `Mac Spy.app` pela pasta Aplicativos.
- **Ainda aparece a versão anterior:** encerre o Mac Spy pelo clique direito e abra novamente.
- **O app foi bloqueado:** use botão direito → **Abrir** ou **Privacidade e Segurança → Abrir Mesmo Assim**.
- **Um processo não pode ser encerrado:** ele provavelmente é protegido pelo macOS ou pertence a outro usuário.

## Integridade do arquivo

SHA-256 do `Mac-Spy-1.4.1.zip`:

```text
4e4d50d6986754214125662b3e437a0fbf331a6e91eb2d3fc32d47c6e5270e8b
```

---

*Dúvidas ou problemas? Abra uma [Issue](../../../issues).*
