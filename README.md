# UC de Bioinformática <img align="right" src="https://github.com/pipapsc/Bioinform-tica---Grupo-6/assets/91962321/efb39dc8-aa19-45a0-b337-ba95fbb5542f" alt="" style="width: 10%; height: 10%;">
<br><br>




### Trabalho realizado por:<br>
```Grupo 6```<br>

PG53810 - Filipa Campos<br>
PG53814 - Francisca Silva<br>
PG53876 - Inês Barroso<br>
PG54186 - Ricardo Barros<br>

<br><br>


## Informação e Descrição do Dataset

<img align="right" src="https://github.com/pipapsc/Bioinform-tica---Grupo-6/assets/91962321/40ce512c-50a5-428f-bd7b-20d2447b9dd1" alt="" style="width: 20%; height: 20%;">

```Dataset 2```: Lung Adenocarcinoma (TCGA, Provisional) <br> 

Link: https://www.cbioportal.org/study?id=luad_tcga <br>

O ficheiro é constituído por dois datasets, o que contém os dados(data_RNA_Seq_v2_expression_median) e o que contém os meta-dados (luad_tcga_clinical_data).

O dataset que contém os dados é constituído por uma coluna Hugo_Symbol cujos valores identificam genes (20531), uma coluna Entrez_Gene_Id que contém o ID de cada gene, e as restantes colunas dizem respeito às amostras (517) relativas a cada paciente (515 pacientes, existindo 2 pacientes que possuem 2 amostras cada um). Cada uma das colunas apresenta quantidades de genes mutados para a amostra em questão.

O dataset dos metadados contém 3 colunas de ID, a primeira do estudo, que é igual para todas as amostras deste dataset, não sendo relevante, a segunda com o ID do paciente e a terceira com o ID da amostra. As restantes colunas dizem respeito a atributos relacionados a doença que contêm dados relativos a cada paciente. <br><br><br>  


Artigo: https://www.ncbi.nlm.nih.gov/pubmed/25079552 <br><br> 

Breve resumo do artigo (Abstract): <br> 

O adenocarcinoma do pulmão é a principal causa de morte por cancro em
todo o mundo. Neste artigo é relatado o perfil molecular de 230 adenocarcinomas pulmonares usando RNA mensageiro, microRNA e sequenciamento de DNA integrado com análises de número de cópia, metilação e proteómica.
Altas taxas de mutação somática foram observadas (médio de 8,9
mutações por megabase). Dezoito genes sofreram mutações estatisticamente
significativas, incluindo mutações de ativação do RIT1 e mutações MGA de
perda de função recentemente descritas que são mutuamente exclusivas com
amplificação focal de MYC. As mutações do EGFR foram mais frequentes em
pacientes do sexo feminino, enquanto as mutações no RBM10 foram mais
comuns nos homens. Aberrações em NF1, MET, ERBB2 e RIT1 ocorreram em
13% dos casos e foram enriquecidas em amostras sem um oncogene ativo,
sugerindo um papel de driver para esses eventos em certos tumores. A
sequência de DNA e mRNA do mesmo tumor destacou alterações de splicing
impulsionadas por alterações genómicas somáticas, incluindo a ausência do
exão 14 no mRNA MET em 4% dos casos. A atividade da via MAPK e PI(3)K,
quando medida no nível da proteína, foi explicada por mutações conhecidas em
apenas uma fração dos casos, sugerindo mecanismos adicionais e inexplicáveis
de ativação da via. Esses dados estabelecem uma base para a classificação de
novas investigações patogénicas moleculares do adenocarcinoma pulmonar.<br><br><br> 



## Objetivo do trabalho



Pretende-se estabelecer uma relação entre dados de expressão genética e meta-dados clínicos sobre pacientes com historial de adenocarninoma pulmonar, um caso específico dentro do Cancro de Pulmão de Células Não Pequenas (NSCLC - Non Small Cells Lung Cancer), visando a previsão da ocorrência ou não de tumor. Identificaram-se também quais os genes e fatores de maior influência nesta doença. A linguagem de programação utilizada para tal foi o Python.<br><br><br>
<p align="center">
  <img src="https://github.com/pipapsc/Bioinform-tica---Grupo-6/assets/91962321/bb00be73-8c87-4f3f-8516-20cb2dabf23c" alt="Adenocarcinoma Pulmonar" style="width:30%; height:30%;">
</p>
<br> <br> 




## Conclusão


Foi possível atingir o principal objetivo do trabalho, que se prende com a previsão de ocorrência ou não de tumor para cada indivíduo. No entanto, os resultados obtidos tanto na aprendizagem não supervisionada como na supervisionada não foram satisfatórios.

O objetivo de se terem realizado 2 versões de dados de entrada para algoritmos de aprendizagem supervisionada foi para avaliar se com mais informação clínica, as previsões seriam mais eficazes, contudo acabaram por ser semelhantes nas duas versões.

A previsão de casos clínicos através de modelos de machine learning acarreta riscos de diagnósticos incorretos (FP e FN), que no caso dos FP podem levar à aplicação de terapias desnecessárias, enquanto nos FN pde resultar no atraso do tratamento e na progressão da doença. Assim, para um diagnóstico ser mais preciso, este deve assentar em múltiplos fatores, para além de se fazer uma maior recolha de dados, nomeadamente de pacientes com tumor. No entanto, é importante evitar aumentar a complexidade do modelo, para este manter a capacidade de generalizar.

O presente dataset não é, portanto, adequado para este tipo de previsões devido às suas características.



