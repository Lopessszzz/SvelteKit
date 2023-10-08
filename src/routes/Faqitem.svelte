<script>
  let questions = [
    {
      question: "O que é a IA Walker?",
      answer: "A IA Walker é um exemplo de resposta que está crescendo acada vez."
    },
    {
      question: "Por que a IA Walker foi criada?",
      answer: "A IA Walker foi criada para fornecer uma plataforma onde as pessoas podem obter facilmente informações atualizadas sobre inteligência artificial."
    },
    {
      question: "Qual a nossa missão, visão e valores?",
      answer: "A IA Walker preza pelo desenvolvimento..."
    },
    {
      question: "Como posso contribuir para a IA walker?",
      answer: "Você pode contribuir enviando suas notícias e artigos relacionados a IA através do link Contribuir em nosso site."
    },
    // Adicione mais perguntas frequentes aqui
  ];

  function toggleAnswer(index) {
    questions[index].isOpen = !questions[index].isOpen;
  }
  function handleKeyPress(event) {
    if (event.key === 'Enter' || event.key === 'Spacebar' || event.key === ' ') {
      toggleAnswer(question);
    }
  }
</script>

<div class="centered-faq">
  <h1><strong>FAQ</strong></h1>
  <ul>
    {#each questions as question, index (question.question)}
      <li class="faq-item">
        <div class="question" on:click={() => toggleAnswer(question)} on:keydown={(e) => handleKeyPress(e)}>
          <span>{question.question}</span>
          <span class:open={question.isOpen}><strong>{"+"}</strong></span>
        </div>
        {#if question.isOpen}
          <div class="answer">{question.answer}</div>
        {/if}
      </li>
    {/each}
  </ul>
</div>
