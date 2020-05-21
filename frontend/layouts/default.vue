<template>
  <div>
    <!-- Main starts -->
    <div role="main" class="container">
      <!-- Header starts -->
      <header role="header" class="d-flex align-items-center p-3 my-3 text-white-50 bg-spring-green rounded box-shadow">
        <img class="mr-3" src="/img/spring-boot-saml.png" alt="" height="48">
        <div class="lh-100">
          <h6 class="mb-0 text-white lh-100">Spring Boot &mdash; SAML 2.0 Service Provider</h6>
          <small>
          <span class="badge badge-light">
            <i class="fas fa-code-branch"></i> github.com/vdenotaris/spring-boot-security-saml-sample/tree/2.3.1.RELEASE
          </span>
          </small>
        </div>
      </header>
      <!-- Header ends -->
      <!-- Content starts -->
      <section role="content" class="my-3 p-3 bg-white rounded box-shadow">
        <nuxt/>
      </section>
      <!-- Content ends -->
      <!-- Footer starts -->
      <footer role="footer">
        <ul class="footer-note">
          <li>
            <i class="far fa-copyright"></i> Copyright 2020 &mdash;
            <i class="fab fa-linkedin"></i>
            <a href="https://www.linkedin.com/in/vdenotaris/">Vincenzo De Notaris</a>
          </li>
          <li>
            <i class="fas fa-balance-scale"></i> Licensed under the
            <a href="https://www.apache.org/licenses/LICENSE-2.0">Apache License, Version 2.0</a>
          </li>
          <li>
            <i class="fab fa-github"></i> GitHub:
            <a href="https://github.com/vdenotaris/spring-boot-security-saml-sample">vdenotaris/spring-boot-security-saml-sample</a>
          </li>
          <li>
            <i class="fab fa-docker"></i> Docker Hub:
            <a href="https://hub.docker.com/r/vdenotaris/spring-saml-sp/">vdenotaris/spring-saml-sp</a>
          </li>
          <li>
            <i class="fab fa-stack-overflow"></i> Get supported on StackOverflow:
            <a href="https://stackoverflow.com/questions/tagged/spring-saml">#spring-saml</a>
          </li>
          <li class="margin-top-10">Wanna say thanks to the developer? <i class="fas fa-beer"></i> <a href="https://beerpay.io/vdenotaris/spring-boot-security-saml-sample">Pay him a beer!</a></li>
        </ul>
      </footer>
      <!-- Footer ends -->
    </div>
    <!-- Main ends -->
    <!-- Bootstrap scripts -->
    <script src="/js/bootstrap.min.js"></script>
    <!-- Font Awesome scripts -->
    <script defer src="https://use.fontawesome.com/releases/v5.0.13/js/all.js"></script>
  </div>
</template>
<script>
export default {
  head() {
    return {
      bodyAttrs: {
        class: 'bg-light'
      }
    }
  }
}
</script>
