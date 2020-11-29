<script>
    export let className = "p-4";
    export let shadow = false;
    export let animation = ''
    export let delay = ''
    export let duration = ''
  </script>
  
  <style>
    .box-shadow {
      -webkit-box-shadow: -9px 11px 22px 0px rgba(0, 0, 0, 0.16);
      -moz-box-shadow: -9px 11px 22px 0px rgba(0, 0, 0, 0.16);
      box-shadow: -9px 11px 22px 0px rgba(0, 0, 0, 0.16);
    }
    .custom-card {
      border-radius: 1rem !important;
      -webkit-transform: translateZ(0);
      transform: translateZ(0);
    }
  </style>
  
  <div data-aos={animation} data-aos-delay={delay} data-aos-duratio={duration} class="card mb-3 custom-card border-0 {shadow ? 'shadow' : ''} ">
    <div class="card-body {className}">
      <slot />
    </div>
  </div>