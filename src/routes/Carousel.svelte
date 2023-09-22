<script lang="ts">
  import {
    Carousel,
    CarouselControl,
    CarouselIndicators,
    CarouselItem,
    CarouselCaption
  } from 'sveltestrap';

  const items = [
    {
      url: 'https://picsum.photos/seed/picsum/536/354',
      title: 'Slide 1',
      subTitle: 'Exemplo 1'
    },
    {
      url: 'https://picsum.photos/id/1084/536/354?grayscale',
      title: 'Slide 2',
      subTitle: 'Exemplo 2'
    },
    {
      url: 'https://picsum.photos/id/870/536/354?grayscale&blur=2',
      title: 'Slide 3',
      subTitle: 'Exemplo 3'
    }
  ];
  let activeIndex = 0;
</script>

<Carousel {items} bind:activeIndex ride interval={2000}>
  <CarouselIndicators bind:activeIndex {items} />

  <div class="carousel-inner">
    {#each items as item, index}
      <CarouselItem bind:activeIndex itemIndex={index}>
        <img src={item.url} class="d-block w-100" alt={item.title} />
        <CarouselCaption
          captionHeader={item.title}
          captionText={item.subTitle}
        />
      </CarouselItem>
    {/each}
  </div>

  <CarouselControl direction="prev" bind:activeIndex {items} />
  <CarouselControl direction="next" bind:activeIndex {items} />
</Carousel>
