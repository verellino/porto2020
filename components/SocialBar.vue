<template>
  <div class="sox">
        <ul>
            <li>
                <a href="mailto:verellino@gmail.com?subject=WASSUP MEKEL!🤙">
                    <fa :icon="faEnvelope" />
                </a>
            </li>
            <li>
                <a href="https://id.linkedin.com/in/michael-verellino-0b99a7142">
                    <fa :icon="faLinkedinIn" />
                </a>
            </li>
            <li>
                <a href="http://behance.com/verellino">
                    <fa :icon="faBehance" />
                </a>
            </li>
            <li>
                <a href="http://twitter.com/verellino">
                    <fa :icon="faTwitter" />
                </a>
            </li>
            <li>
                <a href="http://instagram.com/verellino">
                    <fa :icon="faInstagram" />
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
import { faEnvelope } from '@fortawesome/fontawesome-free-solid'
import { faTwitter, faInstagram, faBehance, faLinkedinIn } from '@fortawesome/free-brands-svg-icons'
export default {
    
    computed: {
      faEnvelope () {
         return faEnvelope
      },
      faTwitter () {
         return faTwitter
      },
      faInstagram () {
         return faInstagram
      },
      faLinkedinIn () {
         return faLinkedinIn
      },
      faBehance () {
         return faBehance
      },
    },
    name: 'SocialBar'
}
</script>

<style>
.sox{
    position: fixed;
    display: flex;
    width: calc(100vw - 160px);
    bottom: 40px;
    justify-content: flex-end;
    z-index: 100;
    mix-blend-mode: difference;
}
.sox ul{
    display: flex;
}
.sox li{
    display: inline-block;
    padding: 0 1rem;
}
</style>