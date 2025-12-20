📌 Backend – API de Validação de Alunos
Esta API é responsável por gerenciar a validação de alunos no momento do login, realizando consultas no banco de dados do projeto para verificar se o aluno já respondeu ou não ao questionário.
O sistema utiliza o Supabase como banco de dados, permitindo identificar se o aluno já possui um registro associado ao seu login.

🎯 Objetivo da API
Garantir que:
Alunos que já responderam o questionário sejam direcionados diretamente para a página de resultados.
Alunos que ainda não responderam sejam direcionados para a página de teste, onde poderão responder ao questionário.
Dessa forma, evita-se que um aluno responda o questionário mais de uma vez, mantendo a integridade dos dados.

🔄 Fluxo de Funcionamento
O aluno realiza o login no sistema.

A API consulta o banco de dados para verificar se:

O aluno já existe no sistema

O questionário já foi respondido.

Com base nessa verificação:

✅ Se já respondeu → o sistema retorna os dados e o aluno é direcionado para a página de resultados, onde são exibidas:


A pontuação final

O curso indicado com base nas respostas

❌ Se não respondeu → o aluno é direcionado para a página de teste para responder o questionário.

Ao final do questionário:

As respostas e o resultado são salvos no banco de dados.

Em acessos futuros, o aluno verá apenas o resultado já calculado, sem necessidade de refazer o questionário.

🛠 Tecnologias Utilizadas
Backend: Python
Framework: FastAPI
Banco de Dados: Supabase
Comunicação: API REST (JSON)

🌐 Integração com o Frontend

A API fornece endpoints que permitem ao frontend:
Validar o login do aluno
Verificar se o questionário já foi respondido
Retornar os dados do resultado quando aplicável
🚀 Deploy

Este backend foi preparado para deploy em ambiente de produção, permitindo integração direta com o frontend do projeto.

🔗 URL da API:https://backend-para-deploy.onrender.com

