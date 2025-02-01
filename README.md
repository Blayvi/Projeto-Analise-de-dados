Esse projeto tem como finalidade analisar de forma objetiva os dados de uma empresa de telecomunicação. 
Foram destacados problemas encontrados por meio dos dados e sugeridas medidas para solucionar os problemas de alto cancelamento na empresa.


# Sugestão de melhora no código do Passo 5 
# comparar cada coluna da minha tabela com a coluna de cancelamento
import plotly.express as px

# etapa 1: criar o gráfico
for coluna in tabela.columns:
    grafico = px.histogram(tabela, x=coluna, color="Churn", text_auto=True)
    grafico.show()
