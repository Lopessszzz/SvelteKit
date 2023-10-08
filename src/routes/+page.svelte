<script>
	// @ts-ignore
	import Badge from './Badge.svelte';
	// @ts-ignore
	import Buttons from './Buttons.svelte';
	// @ts-ignore
	import Header from './Header.svelte';
  // @ts-ignore
  import Button from './Buttons.svelte';
	import Carousel from './Carousel.svelte';
	import Footer from './Footer.svelte';
	import Icons from './Icons.svelte';
  import Faq from './Faqitem.svelte';
	import Support from './Support.svelte';
</script>

<main
    class="content-below-header">
    <Header />


<div>
    <div class="mt-5 padding" > 
        <div class="center-text" >
            <p><strong>IA Walker</strong></p>
			<h6>A inteligência artificial (IA) é uma das áreas mais promissoras. E por isso a IA Walker...</h6>
        </div>
		

        <div class="container">
			  <Carousel />
        </div> 
    </div>
    <div class="columns">
      <div class="column">
      </div>
      <div class="column">
        <Icons />
      </div>
    </div>
    <hr class="div">
    <hr class="div">
    <div class="primary-banner">
        <h1>Experimente um mundo de facilidades!</h1>
        <p>Comece agora mesmo.</p>
        <Buttons />
    </div>
    <Faq />
</div>
</main>

        
			

<Support />

<Footer />
<body />








