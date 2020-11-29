<script>
    import { Card, ContainerFluid } from "../core";

    const cards = [
        {
            title: `Massagem Modeladora`,
            text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cumque, nobis.`,
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
            text: `Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque molestiae deleniti atque aliquam iste odio fugit?`,
        },
        {
            title: "Reflexologia Podal",
            text: `Lorem ipsum dolor sit amet consectetur, adipisicing elit.`,
        },
        {
            title: "Ventosaterapia",
            text: `Lorem ipsum dolor sit amet consectetur adipisicing elit.`,
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

<div class="feature-section" id="features">
    <ContainerFluid style="" p="px-0" height="screen-height">
        <div class="bg-img" style="padding: 5rem 0;">
            <div class="container" data-aos="zoom-in" data-aos-delay="100">
                <h2 class="text-gradient mb-4 text-center">
                    Todo respeito e segurança com seus dados e privacidade.
                </h2>

                <div class="grid feature-section">
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
                                shadow={false}
                                animation="fade-in"
                                delay={(index+1) * 300}
                                className="p-4 py-5">

                                <h4 class="text-uppercase m-0">{card.title}</h4>
                                <hr class="my-4" />
                                <div class="small text-black-50">
                                    {card.text}
                                </div>
                            </Card>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </ContainerFluid>
</div>
