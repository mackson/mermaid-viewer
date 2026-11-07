# Mermaid Viewer

Visualizador de diagramas [Mermaid](https://mermaid.js.org/) em um único arquivo HTML. Editor à esquerda, diagrama à direita, sem build e sem servidor.

## Como usar

Abra `mermaid-viewer.html` no navegador:

```bash
xdg-open mermaid-viewer.html
```

Precisa de internet na primeira carga: o Mermaid 11 vem do jsDelivr via ESM.

## O que faz

| Recurso | Detalhe |
| --- | --- |
| Render ao digitar | debounce de 350 ms; erro de sintaxe aparece em caixa sobre o diagrama |
| Abrir arquivo | botão ou arrastar-e-soltar `.mmd`, `.mermaid`, `.md`, `.markdown`, `.txt` |
| Markdown | extrai os blocos ` ```mermaid ` do arquivo e concatena |
| Exemplos | flowchart, sequence, state, ER, gantt, class |
| Zoom e pan | scroll para zoom no cursor, arrastar para mover, duplo clique para ajustar à tela; pinça no touch |
| Exportar | SVG, ou PNG em 2× com o fundo do tema atual |
| Tema | claro/escuro, sincronizado com o tema do Mermaid |
| Persistência | código, tema e largura do editor ficam no `localStorage` |

## Atalhos

| Atalho | Ação |
| --- | --- |
| `Ctrl/Cmd + Enter` | renderizar agora |
| `Ctrl/Cmd + B` | mostrar/ocultar editor |
| `Tab` | indentar dentro do editor |
| `Esc` | sair da tela cheia |
| Duplo clique no diagrama | ajustar à tela |
