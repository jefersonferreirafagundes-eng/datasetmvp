 MVP Análise de Dados e Boas Práticas

 Nome: JEFERSON FERREIRA FAGUNDES
 Matricula: 4052026000082
 Dataset: student_productivity_distraction_dataset_20000 - extraído da Kaggle

# Descrição do Problema

# Identificar se o uso de redes sociais, games, youtube, nível de stress estão associados
# ao desempenho na nota de exame e também verificar se outras variáveis
# como horas de sono e minutos de exercício colaboram para uma maior produtividade, classificados
# por gênero.
# É comum que o celular e as telas em geral sejam apontadas como causa imediata para o desvio da atenção
# dos alunos em sala de aula e por conseguinte ao seu rendimento escolar. No
# entanto, a literatura contemporânea mostra que essa explicação é insuficiente e reducionista.
# A atenção não é um botão que se liga ou se desliga, mas um sistema cognitivo complexo,
# biologicamente limitado e profundamente sensível ao contexto pedagógico, ambiental e
# emocional.
# Autores da neuropsicologia e da educação indicam que a atenção deve ser compreendida como
# um ecossitema: um conjunto de variáveis interdependentes que inclui fadiga cognitiva,
# desenho curricular, ambiente físico, sentido atribuído ao conteúdo e usos das tecnologias
# digitais.
#
# Hipótese 1 — Uso de redes sociais e desempenho acadêmico
#
# Quanto maior o número de horas gastas em redes sociais, games ou YouTube, menor
# tende a ser a nota final no exame.
#
# analisar com gráfico:
#Tipo: Scatterplot
#Eixo X: horas em redes sociais/games/YouTube
#Eixo Y: nota final do exame
#Separação por gênero
#Esse gráfico permite observar se existe tendência negativa (correlação inversa) entre
# o tempo gasto nessas atividades e o desempenho acadêmico.
#
#Hipótese 2 — Sono e desempenho nas avaliações
#
#Alunos que dormem mais horas por noite tendem a obter notas finais mais altas.
#Como analisar com gráfico:
#Tipo: Scatterplot
#Eixo X: horas de sono
#Eixo Y: nota final
#Separação por gênero
#Esse gráfico permite verificar se existe tendência positiva entre sono adequado e desempenho acadêmico.
#
#Hipótese 3 — Exercício físico e produtividade acadêmica
#
#Alunos que realizam mais minutos de exercício físico por dia apresentam maior produtividade acadêmica (nota final mais alta).
#Como analisar com gráfico:
#Tipo: Scatterplot
#Eixo X: minutos de exercício
#Eixo Y: nota final
#Separação por gênero
#Isso permite observar se existe correlação positiva entre atividade física e desempenho.

# Tipo de Problema

# Este é um problema de classificação supervisionada. Dado um conjunto de informações
# sobre os hábitos de estudo de alunos combinados com os tempos gastos em redes sociais, youtube,
# tefefone, games, vamos verificar as horas de sono e tempo de exercicios para saber se
# alteram as notas finais, reduz o nível de stress e aumenta a pontuação do foco.
#

# Seleção de Dados

# O dataset escolhido é um conjunto de dados amplamente disponível e incluído em bibliotecas
# de aprendizado de máquina no Python.
# Foi realizada uma etapa de seleção de dados excluindo os registros de alunos
# que não desenvolveram nenhuma tarefa.


#  Atributos do Dataset

# O dataset "student_productivity_distraction_dataset_20000.csv" possui 6000 registros. Possui os seguintes atributos:

# student_id,                             - identificação do aluno
# age,                                    - idade
# gender,                                 - sexo
# study_hours_per_day,                    - horas de estudo por dia
# sleep_hours,                            - horas de sono
# phone_usage_hours,                      - horas de uso do celular
# social_media_hours,                     - horas em mídias sociais
# youtube_hours,                          - horas de youtube
# gaming_hours,                           - horas de games
# breaks_per_day,                         - minutos de descanso diário
# coffee_intake_mg,                       - qtde de café ingerida
# exercise_minutes,                       - minutos de exercícios
# assignments_completed,                  - número de tarefas concluídas
# attendance_percentage,                  - percentual de atenção
# stress_level,                           - nível de stress
# focus_score,                            - nível de foco
# final_grade,                            - nota final
# productivity_score                      - score de produtividade
#

# Análise de Dados

# Nesta etapa de Análise de Dados Exploratória (EDA) sobre o dataset "student_productivity_distraction_dataset_20000.csv,
# visamos entender a distribuição, as relações e as características das variáveis, o que é
# crucial para as etapas subsequentes de pré-processamento e modelagem.
# O dataset utilizado possui 6000 registros com 18 informações para cada um, as quais
# utilizaremos parte das mesmas (500 registros) para buscar entender
# a relação descrita nas hipóteses descritas acima.
