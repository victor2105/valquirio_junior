<script>
    import { wpLink, instaLink, phoneNumber, locationLink, email, address } from '../config'
</script>
<style>

    .dark-green-gradient {
        background: rgba(248,249,250,1);
background: -moz-linear-gradient(top, rgba(248,249,250,1) 0%, rgba(91,120,131,1) 68%, rgba(17,60,75,1) 100%);
background: -webkit-gradient(left top, left bottom, color-stop(0%, rgba(248,249,250,1)), color-stop(68%, rgba(91,120,131,1)), color-stop(100%, rgba(17,60,75,1)));
background: -webkit-linear-gradient(top, rgba(248,249,250,1) 0%, rgba(91,120,131,1) 68%, rgba(17,60,75,1) 100%);
background: -o-linear-gradient(top, rgba(248,249,250,1) 0%, rgba(91,120,131,1) 68%, rgba(17,60,75,1) 100%);
background: -ms-linear-gradient(top, rgba(248,249,250,1) 0%, rgba(91,120,131,1) 68%, rgba(17,60,75,1) 100%);
background: linear-gradient(to bottom, rgba(248,249,250,1) 0%, rgba(91,120,131,1) 68%, rgba(17,60,75,1) 100%);
filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f8f9fa', endColorstr='#113c4b', GradientType=0 );
    }

    .dark-green-bg {
        background: #113c4b;
    }
</style>

<section class="signup-section dark-green-bg" id="signup">
    <div class="container">
        <div class="row">
            <div class="col-md-10 col-lg-8 mx-auto text-center">
                <i class="far fa-paper-plane fa-2x mb-2 text-white" />
                <h2 class="text-white mb-5">Inscreva-se para novidades!</h2>
                <form class="form-inline d-flex" action="https://app.us7.list-manage.com/subscribe/post?u=ad98bdfde46053180611f36ab&amp;id=d014c76e31" method="post">
                    <input
                        class="form-control flex-fill mr-0 mr-sm-2 mb-3 mb-sm-0"
                        id="inputEmail"
                        name="EMAIL"
                        type="email"
                        placeholder="Digite o email..." />
                    <button
                        class="btn btn-primary mx-auto"
                        type="submit">Seguir</button>
                </form>
            </div>
        </div>
    </div>
</section>

<section class="contact-section dark-green-bg">
    <div class="container">
        <div class="row">
            <div class="col-md-4 mb-3 mb-md-0">
                <div class="card py-4 h-100">
                    <div class="card-body text-center">
                        <i class="fas fa-map-marked-alt text-primary mb-2" />
                        <h4 class="text-uppercase m-0">Endereço</h4>
                        <hr class="my-4" />
                        <div class="small text-black-50">
                            <a
                                href={locationLink}>
                                {address}
                            </a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-3 mb-md-0">
                <div class="card py-4 h-100">
                    <div class="card-body text-center">
                        <i class="fas fa-envelope text-primary mb-2" />
                        <h4 class="text-uppercase m-0">Email</h4>
                        <hr class="my-4" />
                        <div class="small text-black-50">
                            <a href="#!">{email}</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-3 mb-md-0">
                <div class="card py-4 h-100">
                    <div class="card-body text-center">
                        <i class="fas fa-mobile-alt text-primary mb-2" />
                        <h4 class="text-uppercase m-0">Telefone</h4>
                        <hr class="my-4" />
                        <div class="small text-black-50">
                            {phoneNumber}
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="social d-flex justify-content-center">
            <a
                class="mx-2"
                target="_blank"
                href={wpLink}><i
                    class="fab fa-whatsapp" /></a>
            <a
                class="mx-2"
                target="_blank"
                href={instaLink}><i
                    class="fab fa-instagram" /></a>
            <!-- <a class="mx-2" href="#!"><i class="fab fa-github" /></a> -->
        </div>
    </div>
</section>
<footer class="footer dark-green-bg small text-center text-white-50">
    <div class="container">Copyright © Kiro Mass 2020</div>
</footer>
