# Power BI HTML/CSS Cards Kit

Este repositório contém uma coleção de **5 modelos de cards de indicadores modernos e responsivos** desenvolvidos em HTML e CSS para serem utilizados dentro do Power BI. 

Os cards foram projetados para oferecer uma experiência de interface de utilizador superior à dos visuais nativos, incluindo efeitos de interatividade e adaptação automática a diferentes tamanhos de ecrã.

## Funcionalidades

* **100% Responsivo:** Uso da função CSS e unidades para garantir que o texto e os ícones escalem conforme o tamanho do visual.
* **Interatividade:** Efeito de *Hover* que altera as cores do card ao passar o mouse.
* **Pronto para DAX:** Código otimizado com aspas simples para fácil integração em medidas DAX.
* **Customizável:** Variáveis no topo do código para fácil alteração de cores, títulos e valores.

## Modelos Incluídos

1.  **Card 1 Padrão :** Design minimalista focado na métrica.
2.  **Card 2 com Ícone Central:** Organização vertical com ícone divisor.
3.  **Card 3 com Ícone no Canto:** Foco total no valor com ícone de suporte no topo.
4.  **Card 4 Lateral com Divisor:** Layout horizontal com linha de separação vertical.
5.  **Card 5 Estruturado em "T":** Divisão clara para exibir valor absoluto e percentual lado a lado.

## Como Utilizar

Para utilizar estes cards no seu relatório:

1.  Instale um visual de renderização de HTML no seu Power BI (ex: **HTML Content** ou **HTML VizCreator**).
2.  Crie uma nova **Medida DAX**.
3.  Copie o código de um dos modelos deste repositório e cole na medida.
4.  Substitua as variáveis `vTitulo`, `vValor` ou `vIconeSVG` pelas suas próprias métricas.
5.  Arraste a medida para o campo de dados do visual de HTML.

### Exemplo de Configuração DAX:

```dax
Medida_Exemplo = 
VAR vTitulo = "Vendas Totais"
VAR vValor = FORMAT([Soma_Vendas], "C0")
-- Insira aqui o restante do código HTML/CSS fornecido no repositório
RETURN Template