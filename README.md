# Finacial_Insights

## Especificação Técnica: Insights Interativos Inteligentes
## Para transformar a análise estática em uma experiência interativa inspirada no Power BI, faremos as seguintes atualizações:

## Motor de Insights Estruturados (geminiService.ts):
 - O prompt será ajustado para solicitar ao Gemini uma resposta em formato JSON.
 - Cada insight conterá: Título, Descrição, Tipo (Tendência, Outlier, Padrão) e um Filtro de Ação (segmento, país ou ano específico).

## Painel de Insights Dinâmicos (AIAnalystPage.tsx):
 - Substituição do bloco de texto por uma galeria de Cards Interativos.
 - Cada card terá uma cor temática baseada no tipo de insight (ex: Vermelho para valores atípicos/outliers, Azul para tendências).
 - Adição de um botão "Explorar Dados" em cada insight que, ao ser clicado, aplica automaticamente o filtro correspondente e navega para a visão detalhada.

## Integração de Estado Global (App.tsx):
 - Implementação de uma função handleApplyInsight que recebe os parâmetros sugeridos pela IA e atualiza o estado do dashboard instantaneamente.
## Aprimoramento Visual:
 - Uso de animações suaves para o carregamento dos cards.
 - Indicadores visuais claros (badges) para identificar a natureza do insight.

## Especificação do Novo Design "Midnight Professional"
## Paleta de Cores Base:
- Fundo Principal: Slate 950 (#020617) para profundidade máxima.
- Superfícies (Cards/Header): Slate 900 (#0f172a) com bordas sutis em Slate 800.
- Tipografia: Texto primário em Slate 100 e secundário em Slate 400.

## Paleta de Dados (Harmonia e Contraste):
- Azul Elétrico: #3b82f6 (Vendas)
- Verde Esmeralda: #10b981 (Lucro/Positivo)
- Âmbar: #f59e0b (Alertas/Padrões)
- Violeta: #8b5cf6 (Segmentos Especiais)
- Rosa Vibrante: #f43f5e (Atenção/Outliers)

## Refinamentos Visuais:
- Efeito Glassmorphism: Uso de transparências e borrões sutis em elementos de destaque.
- Gráficos: Eixos e grades em cores suaves (Slate 700/800) para não poluir a visão, permitindo que as cores dos dados saltem aos olhos.
- Interatividade: Hover states com brilho (glow) e transições suaves.
