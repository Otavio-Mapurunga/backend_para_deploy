📌 Backend – API de Validação de Alunos
Esta API é responsável por gerenciar a validação de alunos no momento do login, realizando consultas no banco de dados do projeto para verificar se o aluno já respondeu ou não ao questionário.
O sistema utiliza o Supabase como banco de dados, permitindo identificar se o aluno já possui um registro associado ao seu login.

garantindo que:
Alunos que já responderam o questionário sejam direcionados diretamente para a página de resultados.
Alunos que ainda não responderam sejam direcionados para a página de teste, onde poderão responder ao questionário.
Dessa forma, evita-se que um aluno responda o questionário mais de uma vez, mantendo a integridade dos dados.


🛠 Tecnologias Utilizadas


Backend: Python

Framework: FastAPI

Banco de Dados: Supabase

Comunicação: API REST (JSON)

🚀 Deploy

Este backend foi preparado para deploy em ambiente de produção, permitindo integração direta com o frontend do projeto.

🔗 URL da API:https://backend-para-deploy.onrender.com

O frontend deste projeto pode ser acessado no repositório abaixo:

🔗 https://github.com/LianMary/projetoDeExtensao.git


📚 Documentação Completa

A documentação detalhada do sistema (arquitetura, banco de dados, lógica, casos de uso) está disponível no link abaixo:

https://www.notion.so/Documenta-o-Backend-Sistema-de-Login-Teste-Vocacional-7afa4737f63a45e5b711cd12b0850835?source=copy_link



