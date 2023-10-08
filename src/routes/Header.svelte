<script lang="ts">
  import 'bootstrap/dist/css/bootstrap.min.css';
  import "./Styles.css" 
  import { Button, Modal } from 'sveltestrap';
  let isOpen = false;
  const toggle = () => (isOpen = !isOpen);
</script>

<nav class="navbar navbar-expand-lg bg-body-tertiary fixed-header" style="height: 90px;">
    <div class="container-fluid">
      <a class="navbar-brand text-primary" href="/">
        <img src="https://media.licdn.com/dms/image/C4D0BAQHD26P4n6f_-g/company-logo_200_200/0/1662026081450?e=1704326400&v=beta&t=JMQNMQj38_CynnJ8ZNv_rldX_FmlehieLPkuDu2EDOk" alt="Ícone" width="50" height="50"> 
        <span class="ml-2" style="font-size: 30px;"><strong>IA Walker</strong></span>
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDarkDropdown" aria-controls="navbarNavDarkDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav mx-auto">
          <li class="nav-item">
            <button class="btn btn dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false" style="font-size: 19px;">
              Produtos
            </button>
            <ul class="dropdown-menu dropdown-menu multi-column" aria-labelledby="produtosDropdowns">
              <li>
                  <div class="container">
                      <div class="row">
                          <div class="col">
                              <h5 class="dropdown-header">Categoria 1</h5>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 1</a>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 2</a>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 3</a>
                          </div>
                          <div class="col">
                              <h5 class="dropdown-header">Categoria 2</h5>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 4</a>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 5</a>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 6</a>
                          </div>
                          <div class="col">
                              <h6 class="dropdown-header">Categoria 3</h6>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 7</a>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 8</a>
                              <a class="dropdown-item" href="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg">Produto 9</a>
                          </div>
                      </div>
                  </div>
              </li>
          </ul>
          <li class="nav-item">
            <a class="nav-link" href="/catalog" style="font-size: 18px;">Catálogo</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/catalog" style="font-size: 18px;">Sobre o projeto
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="https://www.google.com/">Action</a></li>
            </ul>
          </li>
        </ul>
        <ul class="navbar-nav ms-auto d-flex"> 
          <li class="nav-item" style="font-size: 26px;">
            <Button color="white" on:click={toggle}>Contato</Button>
            <Modal body {isOpen} {toggle} header="Contato">
              <p>Entre em contato conosco através dos canais abaixo:</p>
              <img
              src="https://i.ytimg.com/vi/NUJIRujygvY/hqdefault.jpg"
              alt="Come on Get Happy"
              class="img-fluid"
              />
            </Modal>
          </li>
          <li class="nav-item">
            <a class="nav-link botao-sem-hover" href="/login" style="font-size: 20px;">
              <strong>Login</strong></a>
          </li>
        </ul>
      </div>
    </div>
</nav>
