<script>
    import { Card, ContainerFluid } from "../core";

    const cards = [
        {
            title: `Massagem Modeladora`,
            text: ``,
        },
        {
            title: `Drenagem Linfática`,
            text: `Oferecemos tanto drenagens linfáticas direcionadas quanto de corpo inteiro`,
        },
        {
            title: `Massagem Relaxante`,
            text: `Oferecemos tanto massagens relaxates direcionadas quanto de corpo inteiro`,
        },
        {
            title: `Massagem Facial`,
            text: ``,
        },
        {
            title: "Reflexologia Podal",
            text: ``,
        },
        {
            title: "Ventosaterapia",
            text: ``,
        },
    ];
</script>

<style>
    .grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 2em;
    }
    .bg-img {
        position: relative;
        overflow: hidden;
    }
    .bg-img img {
        position: absolute;
        right: -50%;
        max-height: 100%;
    }
</style>

<div id="features">
    <ContainerFluid style="" p="px-0" height="screen-height">
        <div class="bg-img">
            <img
                loading="lazy"
                alt="bg"
                src="svgs/imagens-ora-consorcio_parceiro-carro-background.svg" />

            <div class="container" data-aos="zoom-in" data-aos-delay="100">
                <h2 class="text-gradient mb-4">
                    Todo respeito e segurança com seus dados e privacidade.
                </h2>

                <div class="grid">
                    {#each cards as card, index}
                        <div
                            style="display: grid;"
                            on:mouseenter={() => {
                                cards[index].hover = true;
                            }}
                            on:mouseleave={() => {
                                cards[index].hover = false;
                            }}>
                            <Card
                                shadow={card.hover}
                                animation="fade-in"
                                delay={index * 200}
                                className="p-4 py-5">
                                <h4 class="text-primary">{card.title}</h4>
                                <p class="mt-4">{card.text}</p>
                            </Card>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </ContainerFluid>
</div>
