<script>
    export let icons = [
      {
        name: 'Facebook',
        iconUrl: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAOEAAADhCAMAAAAJbSJIAAAAaVBMVEVIWpb///80So7s7fNCVZR7hq9GWJVOX5nz9PhfbaE3TY9AVJM5TpDX2uVRYprQ0+FwfKlYZ52bo8GzuM8uRozj5e3IzNy9wtWsssuRmruDjbOgp8Tw8fXa3eelrMeHkbZmdKRteqgYN4aJcfDyAAAD4UlEQVR4nO3dbXOiMBSG4UDZFJPIa9DWRdvu//+Ri1JnutNZGsXknGSe+0s/leEahCABFNlndddUIpWqpquvMDH/6bXSUlKv2MOScvL0X4Rja6jXyUOmHa/CQRXUa+MlqYZZOKp0Pp7/JtV4EbZpbsFzRXsW9inug9dMPwk19Vp4TWeiVtQr4TVViy7xbdiJJtUD6ZxsRJW4MJ1TUYQQQgghhBBCCCGE7kwW2qg8z22upj/W5peUUsZorYsi7muEUitbHU777VBmXyrHp+FY7/b9qXtrNsXkjZNZGPt+2mYOlUOMW1LbZl/+jPssuolBaeSLOy9Coar2t/CiE+riVl9cQmm7m31RCfXzcAcwIqE63OOLSGhf7gNGI7S7O4GxCG39MyVq4QpgHML89lEwLqG5ZxiMSVi8rwFGIJTqphPtCIX53eNEJMKiWQfkL7RPiQv160oge6Fdd5jhL1y/CbkLV++F3IWrD6TshWblWMheKNV6IG9h8Za68BEfUt7C9YMhc6HcPADIWqhv/OZbDsftt46cn5m8ZTfcvW7mydFvMQaK3PWEZjhYozlL/lfuCOws531tIdcDzXu0zw46jvcf8T53pn+7APuIHx00vYswj/EI85nTYBH1A7zK5XaSTcSbUKijg9BSr+WacodJ7W3Exxm3U5qod0Mn4e94B0PhJnxNXniI9Ix0zkX4C0LWQQgh/yCEkH8QQsg/CCHkH4QQ8g9CCPmXhlAu5CTUS0uQDO5SeF7IuAgXlzBF/E7Ex9wws9iYpy4kfrtsAOGeduomgJB46iaAkHhiI4CQeBY8gNCkLixpB4sAwoF4nt+/cEc8z+9f2BPPgvsXUr9O3r+Q+tuVf2FL/PXJv5B4sPAvpB4O/QuP1Le9eRdSD4f+hS/UN4V5F5Lf9uZd2FBfbPQufKa+muhdSH6PtG/hE/Vw6F1Ifxe4byHxpcQAwhP1YOFd+Ja88IN6sPAupB7v/QvJh0PfQvrh0LeQwe82TsJyIQfE0r+X1JcSL8R8oT8Os9yNXVgAA+ByadyLsRSEEPIPQgj5ByGE/IMQQv5BCCH/IISQfxBCyD8IIeQfhBDyD0II+QchhPyDEEL+QQgh/yCEkH8QQsg/CCHkH4QQ8g9CCPkHIYT8gxBC/kEIIf8ghJB/EELIPwgh5F9AYUXzIptQQlmJJnFhI4hexhtKqDtB9J6XUEJViyzxbZgJot/3DiQ0/STMWophJ4ywaLOzcFQEh9MgQqnGizAbVPitGEJYqCGbhdnYBt8XAwhNO2ZX4fkl/EoH/YUov0IpJ08/L0VcF1d3TcgfiPIrrJquvi7lL/eDSV3Karp8AAAAAElFTkSuQmCC', // Substitua pela URL do ícone do Facebook
        link: 'URL_DO_LINK_DO_FACEBOOK', // Substitua pela URL do seu perfil do Facebook
      },
      {
        name: 'IA NEWS',
        iconUrl: 'https://ianews.app/image/logo-no-bg.png', // Substitua pela URL do ícone do Twitter
        link: 'https://ianews.app/', // Substitua pela URL do seu perfil do Twitter
      },
      {
        name: 'Instagram',
        iconUrl: 'https://imagepng.org/wp-content/uploads/2017/08/instagram-icone-icon-1.png', // Substitua pela URL do ícone do Instagram
        link: 'https://www.instagram.com/walker_design_implementacao/', // Substitua pela URL do seu perfil do Instagram
      },
      {
        name: 'LinkedIn',
        iconUrl: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTPRPh7V9bwKzF34_7YkYzM-qozQ6Wyft_2UA&usqp=CAU', // Substitua pela URL do ícone do LinkedIn
        link: 'https://www.linkedin.com/', // Substitua pela URL do seu perfil do LinkedIn
      },
    ];
  </script>
  
  <div class="social-icons">
    {#each icons as icon}
      <a href={icon.link} target="_blank" rel="noopener noreferrer">
        <img src={icon.iconUrl} alt={icon.name} />
      </a>
    {/each}
  </div>