# Relatório de desenvolvimento — Blood Moon

## 1. Repositório e execução

**Repositório:** https://github.com/5g8p6bzzxf-crypto/blood-moon

O projeto é uma aplicação web estática feita com HTML, CSS e JavaScript, sem instalação de dependências.

### Executar localmente
1. Baixe o projeto pelo botão **Code → Download ZIP** do GitHub e extraia os arquivos.
2. Abra `index.html` em um navegador atualizado.

Como alternativa, abra um terminal na pasta do projeto e execute:

```bash
python -m http.server 8000
```

Depois, acesse http://localhost:8000.

### Publicar com GitHub Pages
No repositório, abra **Settings → Pages**. Em *Build and deployment*, escolha **Deploy from a branch**, selecione a branch `main` e a pasta `/(root)`, e clique em **Save**. Aguarde a publicação e abra o endereço indicado pelo próprio GitHub.

## 2. Funcionalidades implementadas

- Catálogo com oito fases: Lua Nova, Crescente Inicial, Quarto Crescente, Gibosa Crescente, Lua Cheia, Gibosa Minguante, Quarto Minguante e Minguante Final.
- Seleção das fases com nome, descrição, iluminação aproximada e dia estimado do ciclo.
- Simulador didático de um ciclo lunar de aproximadamente 29,5 dias, com iniciar, pausar, continuar, reiniciar e seleção de velocidade.
- Quiz com oito perguntas, quatro alternativas por pergunta, feedback, pontuação e opção de tentar novamente.
- Interface responsiva para telas menores.

## 3. Como a IA foi utilizada

A IA foi usada como assistente de desenvolvimento para estruturar a aplicação, escrever e revisar HTML/CSS/JavaScript, explicar os passos de publicação no GitHub e investigar problemas visuais relatados durante a revisão.

**Importante:** este relatório descreve a assistência recebida nesta conversa. Se a atividade exigir especificamente o Google Antigravity, informe separadamente se também utilizou essa ferramenta; não declare seu uso caso não tenha utilizado.

### Exemplos de prompts empregados ou representativos do trabalho realizado

Os exemplos abaixo resumem os pedidos feitos durante o desenvolvimento. Para uma entrega acadêmica rigorosa, substitua-os ou complemente-os com o texto exato dos prompts que você realmente enviou às ferramentas:

1. “Crie uma aplicação web sobre as fases da Lua com interface moderna, oito fases selecionáveis, nome e descrição de cada fase.”
2. “Implemente um simulador do ciclo lunar de aproximadamente 29,5 dias, com iniciar, pausar, reiniciar e controle de velocidade.”
3. “Adicione um quiz com pelo menos cinco perguntas, quatro alternativas, feedback, pontuação e opção de tentar novamente.”
4. “Confira a representação visual das fases, pois algumas luas estão aparecendo iguais.”
5. “Corrija o CSS para que Quarto Crescente, Lua Cheia e Quarto Minguante tenham aparências distintas.”

## 4. Dificuldades encontradas e correções realizadas

- **Representação visual repetida das fases:** foi identificado que o posicionamento da sombra em CSS não distinguia adequadamente todas as fases. O CSS foi ajustado em commits posteriores para alterar a iluminação aparente.
- **Quarto Minguante parecido com Lua Cheia:** foram feitas novas tentativas de ajuste na regra CSS. A alteração mais recente está no histórico do repositório, mas a aparência final ainda deve ser confirmada visualmente no navegador; não considerar o problema resolvido sem essa verificação.
- **Publicação e atualização:** foi necessário orientar a configuração do GitHub Pages e a atualização forçada do navegador para evitar que o cache mostre uma versão anterior.

## 5. Evidências e testes de aceite

Não foram anexadas capturas de tela automaticamente neste relatório. Para demonstrar o funcionamento, tire capturas reais da aplicação executando no navegador e adicione-as ao relatório ou ao repositório.

Sugestões de evidências:
- **Evidência 1 — Fases lunares:** mostrar a grade com as oito fases e uma fase selecionada com descrição.
- **Evidência 2 — Navegação:** mostrar o nome e a ilustração mudando ao usar os botões anterior/próxima.
- **Evidência 3 — Simulador:** mostrar o simulador em execução com contador de dias e controles.
- **Evidência 4 — Quiz:** mostrar uma pergunta com quatro alternativas e, em outra captura, o feedback após responder.
- **Evidência 5 — Resultado:** mostrar a pontuação final e o botão de nova tentativa.
- **Evidência 6 — Responsividade:** mostrar a página em uma janela estreita ou em um celular.

Registre os resultados em [Plano de validação](validacao.md). Marque um requisito como **Aprovado** somente depois de executar o teste correspondente. Se encontrar falha, anote o comportamento observado, corrija e teste novamente.

## 6. Limitações conhecidas

A ilustração lunar é uma representação didática em CSS, não uma simulação astronômica tridimensional precisa. Os dias e percentuais de iluminação são aproximados. Antes da entrega, verifique especialmente a aparência dos quartos crescente e minguante em todos os tamanhos de tela.

## 7. Conclusão

O projeto reúne conteúdo informativo, simulação interativa e avaliação de conhecimentos em uma única página web. A entrega final deve incluir o link do repositório, as evidências reais de teste e o registro fiel das ferramentas e prompts utilizados.
